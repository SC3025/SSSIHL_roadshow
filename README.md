In this one-day workshop, I had the opportunity to explore the exciting fields of VLSI (Very Large Scale Integration) and RISC-V architecture. I learned about the chip manufacturing process and examined different types of chips and microprocessors. This experience was highly valuable, enhancing my knowledge of VLSI and chip design, and broadening my potential career paths in this area.
After opening Virtual Box we opened a new terminal where we wrote our new commands to install gedit

We use the command ### Example Commands to clone a Git repository and install gedit:

 sudo apt install gedit

The password provided by the host was used to install gedit
he new white interface was used to write our code and save it.

Code
  #include<stdio.h>
int main(){
    int sum = 0, i, n;
    printf("Enter the value of n = ");
    scanf("%d",&n);
    for(i = 1;i <= n;i++){
       sum = sum + i;
    }
    printf("The Sum of numbers from 1 to %d is %d\n",n,sum);
    return 0;
}
This was a simple code which adds the number from 1 to n where 'n' is the number provided by us.

After saving the file we opened the previous terminal where we executed the code

we used two commands here

 gcc {file name}.c

./a.out

After running the code we provided the number and it gave the sum of 1 to n.



Then as we are using RISC-V architecture we will use the following command to do so :##
`riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o {filename}.o {filename}.c`
Then we disassemble the file for the RISC-V architecture using the following command :

iscv64-unknown-elf-objdump -d {filename}.o




Working a code on the VSD squadron
After all the designing part we finally got the boards, now it was time to run a code on this board.

We opened VS code where we used the Platform IO extension to run the code which was given to us on Slack.
We then connected the board to to our laptop



