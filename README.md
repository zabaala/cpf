# Gerador de CPF
Classe em PHP para geração dinâmica de CPFs válidos. Esta classe foi criada baseada no algorítmo disponível aqui: http://www.geradorcpf.com/algoritmo_do_cpf.htm.

#Utilização

### Criando um CPF
Criando um cpf com um número aleatório gerado pela classe.
```
$cpf = (new Cpf)->create();
```
Criando um dígito verificador para um CPF de número aleatório informado pelo usuário. Se for informado um CPF válido, a classe irá retornar o dígito verificador real do CPF.
```
$cpf = (new Cpf('111.444.777'))->create();
```
### Validando um CPF
```
$cpf = (new Cpf('000.000.001-91'))->validate(); // retorna true
$cpf = (new Cpf('000.000.001-90'))->validate(); // retorna false
```

#Autor
Mauricio Rodrigues <mauricio.vsr@gmail.com>

#Licença
MIT License (MIT)

Copyright (c) 2016 Mauricio Rodrigues

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


