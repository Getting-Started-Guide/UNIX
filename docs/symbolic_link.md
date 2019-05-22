### Guide

#### Requirements

sudo chmod 700 {/path/to/file-name}

#### Commands

Creation -> ln -s {/path/to/file-name} {/usr/bin/link-name}

Update   -> ln -sfn {/path/to/file-name} {/usr/bin/link-name}

Deletion -> unlink {link-name}
            rm {link-name}

View     -> ls -l {/path/to/file-name}
