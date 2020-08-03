#!/usr/bin/env bash
usage="$(basename "$0") OPTIONS [path] -- display ordered directory sizes

OPTIONS:
    -h          Show this help message

FUNCTION:
    path        Directory path to use as root dir, default current directory
"
usage() {
    echo "$usage"
    exit 1
}

while getopts ':h' option; do
    case "$option" in
        h) usage;;
        \?) printf "illegal option: -%s\n" "$OPTARG" >&2; usage;;
    esac
done

if [ $OPTIND -gt 1 ]; then shift $((OPTIND - 1)); fi
if [ $# -gt 1 ]; then usage; fi

#

if [ ! -z "$1" ]; then
	du -h -d0 $1/* | sort -hr
else
	du -h -d0 ./* | sort -hr
fi

exit $?
