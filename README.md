# Scripts and Aliases used for TWB

## Remove spaces from filenames
`alias twb_remove_spaces='for f in *\ *; do mv "$f" "${f// /_}"; done'`

## Re-encode mp3s to make them smaller in size
`alias twb_re-encode_mp3s='for file in *.mp3; do mv $file orig_${file}; lame -b 56 orig_${file} $file; done'`
