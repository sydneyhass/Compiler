# Compiler
The application contained here makes up the front-end of a compiler. The development for this included the creation of a buffer, scanner, and parser that were responsible for translating a language called **Platypus**.

## Buffer
> *A device or memory area used to store data temporarily and deliver it at a rate different from that at which is was received*

Buffers are commonly used in the implementation of a compiler becuase of their efficiency. The buffer can be operated in any of the following modes: 
- fixed-size
- additive self-incrementing
- multiplicative self-incrementing

The buffer is made up of two associated data structures:
- Buffer Descriptor / Buffer Handle
- Array of Characters

### Buffer Descriptor (Buffer Handle)
The buffer descriptor is responible for holding all of the information about the array of characters. This includes: a pointer to the beginning of the character array in memory, the current capacity, the next charcter entry position, the increment factor, the operational mode, and additional parameters.

## Scanner
The Scanner is is the inital component of the front-end for the compiler. The scanner reads a source program from a text file and produces a stream of token representations. 

The input into the lexical analyzer is the stream of characters contained in the buffer. The output of the scanner is a token representation of a single character or pattern of characters.

The scanner is a mix between a token-driven and table-driven (DFA) scanner. The transition-table part of the scanner is used to recognize variable identifiers, keywords, integer literals, and floating-point literals. 

### Transition Table
<img></img>

## Parser
