#1
`wc -l test_command.gtf`
`wc -c test_command.gtf`
#2
`grep "^chr_" test_command.gtf | grep "YDL248W"`
#3
`sed 's/chr_/chromosome_/g' test_command.gtf | cut -f 1,3,4,5`
#4
`awk '{temp = $2; $2 = $3; $3 = temp; print $0}' test_command.gtf | sort -k 4,5 -n > result.gtf`
#5
`ls -hl`
`chmod 774 test_command.gtf`
`ls -hl`

