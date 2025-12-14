# Lambda Expression

1. Lambda expression is a short way to write anonymous inner class (functions without name)
2. Enables functional programming

Before Java 8 :
----------------------------------------------------
Runnable runnable = new Runnable ({
        @Override
        public void run(){
            System.out.println("Thread is running");
        }
});

After Java 8 :
----------------------------------------------------
Runnable runnable = () -> System.out.println("Thread is running");


Syntax :
----------------------------------------------------
1. without input parameters
() -> { body };

2. with input parameters
(parameters) -> { body with use of parameters };



