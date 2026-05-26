\# Revisão do curso Git \& GitHub do professor Téo Me why.
Link do curso grátis do professor Téo, é grátis:
[Curso Git & GitHub 2025](https://www.youtube.com/watch?v=M-mBmYj7Jh4&list=PLvlkVRRKOYFQyKmdrassLNxkzSMM6tcSL&index=7)

🔗 HTTPS — A forma do print (mais simples para começar)

Funciona como entrar num site qualquer: você usa seu usuário e senha (ou um token que o GitHub gera pra você).

Como é na prática:

Toda vez que você enviar código, ele pode pedir sua senha

Funciona em qualquer computador, qualquer lugar

Não precisa de nenhuma configuração especial

Analogia: É como entrar numa conta de e-mail num computador público — funciona, mas você digita a senha sempre.

🔑 SSH — A forma mais automática

Em vez de senha, você cria uma espécie de "chave única" no seu computador. O GitHub guarda uma cópia dessa chave e passa a reconhecer seu notebook automaticamente — sem pedir senha toda vez.

Como é na prática:

Você configura uma vez só

Depois disso, nunca mais digita senha

Porém: só funciona no computador onde você criou a chave

Analogia: É como ter uma chave física da sua casa. Quem tem a chave entra sem precisar falar nada. Mas essa chave só existe naquele chaveiro específico.

Qual é melhor para você agora?

HTTPSSSHDificuldade pra configurarFácil ✅MédioPede senha toda vez?Às vezesNãoFunciona em qualquer PC?Sim ✅NãoBom pra iniciante?Sim ✅Depois

Recomendação: Como você está começando, siga com o HTTPS como o professor mostrou. Quando você já estiver mais confortável com Git e GitHub no geral, aí vale aprender SSH — principalmente se você usar sempre o mesmo computador.

O professor estava certo: SSH é mais prático no dia a dia, mas exige uma configuração inicial que faz mais sentido depois que você já entende o básico.

#Git Flow
É uma convenção de branches para organizar o desenvolvimento de software com Git.
Branches principais
BranchPapelmainCódigo em produção, estáveldevelopCódigo em desenvolvimento, integração contínua
Branches de suporte

feature/* — novas funcionalidades, criadas a partir da develop
release/* — preparação para uma nova versão, saem da develop e vão para main
hotfix/* — correções urgentes em produção, saem da main e voltam para main e develop


A branch develop
É o coração do desenvolvimento ativo. Funciona como uma área de integração onde todas as features concluídas são mescladas antes de irem para produção.

Toda feature nasce dela e volta para ela via merge
Quando o código está estável e pronto para lançar, uma release é criada a partir dela
Nunca deve ter código quebrado — é a "produção dos desenvolvedores"
