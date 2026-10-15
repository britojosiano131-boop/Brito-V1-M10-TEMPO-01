# BRITO V1 — MATRIZ 10
## Extensão exploratória matéria–tempo: congelamento integral

Data: 15/10/2026 (America/Sao_Paulo).
Estado: deduções condicionais e hipóteses exploratórias preservadas para continuidade. Congelamento documental, não validação experimental.
Autorização: “Vamos congelar e guardar tudo.”

## 1. Escopo e integridade

Este documento consolida toda a frente exploratória desenvolvida nesta conversa: fonte material, atraso, núcleo exponencial, esfera finita, simetria, fase, amplitude e bloco homogêneo. As correções posteriores prevalecem sobre interpretações anteriores.

Não altera a M10-TEMPO-01 congelada em 13/10/2026, a PCB V3.5, o firmware R11 ou outros checkpoints. Não autoriza mudanças de hardware, firmware ou publicação externa.

Fundamentos preservados: 10,1 − 0,1 = 10; 333 − 137 = 196; √196 = 14. Constante rho = 3/140. Cadeia conceitual do projeto: Matéria → Gravidade → Tempo → Luz. Preservar esses fundamentos não equivale a deduzir deles os novos núcleos ou parâmetros.

Fonte consultada: BRITO_V1_M10_TEMPO_01_ANALISE_HORIZONTAL_CONGELAMENTO_2026-10-13.md, identidade libfile_ca2d80ae99fc819184666fb2580a9d30.

## 2. Questão inicial: mudança no Sol

Separar cessação da emissão luminosa, mantendo a distribuição material, de mudança na própria distribuição material. Uma extensão dependente exclusivamente da matéria não prevê mudança temporal decorrente apenas de apagar a emissão com a mesma fonte material. Isso é consequência da hipótese, não demonstração física sobre luz ou gravidade.

A formulação congelada não estabelece acoplamento quantitativo solar nem velocidade de propagação. Os 20 s representam o período diferencial de 0,05 Hz, não tempo de viagem Sol–Terra. Nenhum valor de velocidade foi fixado, inclusive nenhuma igualdade ou desigualdade com a velocidade da luz. Não foi realizada comparação externa nesta frente.

## 3. Resposta material retardada proposta

Theta = 1 + F10[mu] é uma representação a completar, não uma lei derivada.

Para pequenas perturbações, propôs-se:

    deltaTheta(x,t) = integral K10(x,x') deltaMu(x', t − T10(|x−x'|)) dV'

mu representa densidade de massa, em kg/m³; deltaTheta é adimensional; K10 tem unidade kg⁻¹. Essa unidade não exige massa fundamental nem dependência inversa da massa física da fonte.

Parametrização exploratória:

    K10(r) = s alpha/M* f(r/ell)
    s = −1 ou +1; alpha >= 0; M* > 0; ell > 0
    T10(r) = r/v10; 0 < v10 < infinito

M* é referência de massa, ell é alcance, alpha é adimensional. Intensidade, alcance, sinal e velocidade permanecem desconhecidos. O atraso impõe resposta retardada nesta prescrição, sem constituir dinâmica completa.

Escolha postulada: f(r/ell) = exp(−r/ell). É exponencial radial pura, não o núcleo usual de Yukawa, que inclui 1/r. Valores relativos em r/ell = 0, 1, 3, 5: 1; 0,3679; 0,0498; 0,0067. Não há corte espacial abrupto.

Sinal negativo reduz a taxa em relação à base; positivo aumenta. O sinal isolado não estabelece estabilidade. deltaTheta negativo não implica Theta < 1. Exigir Theta = Theta_base + deltaTheta > 0, ou deltaTheta > −Theta_base.

## 4. Fonte pontual e transição

Fonte estática: deltaMu(x') = M0 delta^(3)(x'). Com B = alpha M0/M*:

    deltaTheta(r) = s B exp(−r/ell)

Fonte ideal ligada em t0:

    deltaTheta(r,t) = s B exp(−r/ell) H(t−t0−r/v10)

Chegada: t0+r/v10. Essa prescrição ideal não fornece mecanismo de criação de matéria. O degrau tem derivada singular; o perfil pontual tem direção do gradiente indefinida na origem, sem necessariamente divergência em magnitude.

Se Theta_b for constante e adotarmos adicionalmente a lei candidata a = −KT grad ln Theta, então, para r > 0 e fora da frente:

    a_r = s KT B exp(−r/ell) / [ell (Theta_b+sB exp(−r/ell))]

KT tem unidade m²/s² e valor e sinal ainda abertos. Para KT > 0, B > 0 e Theta > 0, s = −1 dá direção central; s = +1 dá direção externa. Trata-se de resposta candidata sob lei assumida.

## 5. Esfera uniforme finita e transição suave

Raio R > 0, massa M0, densidade mu0 = 3M0/(4 pi R³). Definir tau > 0 e:

    S(u)=0 para u<=0
    S(u)=3u²−2u³ para 0<u<1
    S(u)=1 para u>=1

S possui primeira derivada contínua e limitada; não se afirmou suavidade de todas as ordens.

    deltaMu(x',t)=mu0 indicador(|x'|<=R) S((t−t0)/tau)

    deltaTheta(x,t) = s alpha mu0/M* integral_{|x'|<=R}
      exp(−d/ell) S((t−t0−d/v10)/tau) dV', d=|x−x'|

É uma mudança idealizada de fonte; o processo material correspondente segue aberto. Por simetria, grad Theta(0,t)=0 com base espacialmente constante.

Para r=|x|, o limite inicial de resposta é t0+max(0,r−R)/v10; toda a contribuição está estabelecida em t0+(r+R)/v10+tau. No instante inicial exato S ainda pode ser zero; o marco indica início do suporte temporal.

## 6. Centro estacionário e positividade

Com q=R/ell e B=alpha M0/M*:

    deltaTheta(0)=s B (3/q³)[2−exp(−q)(q²+2q+2)]

Para M0 fixo: q→0 dá sB; q grande dá aproximadamente 6sB(ell/R)³. São limites do núcleo escolhido.

Taxa central candidata pode mudar enquanto o gradiente central é zero. Isso não é medida de relógio real.

Para base constante Theta_b > 0, s = −1 e esta fonte não negativa, B < Theta_b é condição suficiente de positividade em todo o espaço e durante a transição, pois 0 <= exp(−d/ell) S <= 1. Não é necessariamente a condição mais ampla possível.

## 7. Perfil radial estacionário completo

    FR(r) = 3/(4 pi R³) integral_{|x'|<=R} exp(−|x−x'|/ell) dV'
    Theta(r)=Theta_b+s B FR(r)

Para r > 0, redução exata a uma integral:

    FR(r)=3ell/(2R³r) integral_0^R a [
       (|r−a|+ell) exp(−|r−a|/ell)
       −(r+a+ell) exp(−(r+a)/ell)] da

    a_r(r)=−s KT B FR'(r)/(Theta_b+s B FR(r))

FR é radial decrescente; FR'(0)=0; FR→0 no infinito. Não há salto de Theta ou da aceleração candidata na superfície r=R, com positividade. Para KT > 0, B > 0, sinal negativo aponta ao centro e positivo para fora.

## 8. Centro de massa e autointeração

    a_CM = (1/M0) integral_V mu a dV

No caso esférico simétrico, base constante e campo radial, a_CM=0 por cancelamento direcional. Isso significa ausência da aceleração resultante atribuída ao campo, não obrigação de repouso: velocidade constante também é possível.

Assimetria remove um argumento de simetria, mas não garante resultante não nula. Para campo próprio, a integral material deve ser analisada junto à dinâmica da fonte, campo, atuadores e ambiente. Para campo externo prescrito, calcula-se a resposta do corpo ao campo imposto. Esses casos não são intercambiáveis.

Nenhum relato de bancada foi auditado ou identificado como evidência de mecanismo temporal nesta conversa. Compatibilidade com cancelamento simétrico não identifica sua causa.

## 9. Campo oscilatório congelado: fase e amplitude

    Theta(x,t)=1+rho tanh[A(x) sin psi]
    psi=2 pi (0,05)t+phi(x); rho=3/140

A e phi fixos no tempo, média de ciclo completo de 20 s, geometria e densidade fixas. Derivada:

    grad ln Theta = rho sech²(A sin psi)/(1+rho tanh(A sin psi))
       [sin psi grad A + A cos psi grad phi]

Definir a média logarítmica, usando a letra script L para evitar confusão com comprimento:

    Lcal(A)=1/(2pi) integral_0^(2pi) ln[1+rho tanh(A sin u)] du
           =1/(4pi) integral_0^(2pi) ln[1−rho² tanh²(A sin u)] du

A média independe da fase fixa. O cancelamento não se justifica apenas pela integral isolada do cosseno, pois há fatores multiplicativos; justifica-se pela invariância da média periódica sob deslocamento de fase.

    <a>=−KT Lcal'(A) grad A

Para A>0, Lcal'(A)<0. Com KT>0, a resposta média local aponta para amplitude maior. Amplitude espacialmente constante implica média local nula, mesmo com gradiente de fase. Essa afirmação não inclui fase/amplitude variáveis no tempo, geometria móvel ou janelas incompletas.

Pequena amplitude:

    Lcal(A) ≈ −rho² A²/4
    <a> ≈ (9/78400) KT grad(A²)
    <a_x> ≈ (9/39200) KT A A'

A não linearidade já fornece essa retificação candidata; ela não assegura resultante global.

## 10. Fronteiras, homogeneidade e correção de integração por partes

    integral_V mu grad(A²) dV
      = integral_borda mu A² n dS − integral_V A² grad mu dV

Isolamento não elimina automaticamente o termo de superfície. Em um corpo homogêneo finito ele pode ser toda a contribuição. Em integral sobre todo o espaço, a variação de densidade na borda deve ser incluída, em sentido distribucional se abrupta.

Logo, gradiente de densidade no interior não é necessário para resultante candidata não nula em um campo prescrito. Também não se deduz dos relatos experimentais que esse seja o mecanismo presente.

## 11. Marco exato: bloco homogêneo em campo prescrito

Hipóteses: densidade mu0 e seção transversal S constantes; comprimento L>0; M=mu0 S L; KT constante; Theta com base 1 da equação oscilatória; A=A(z) e fase espacial fixas no tempo; campo regular; média de ciclo completo; corpo e geometria tratados fixos na avaliação.

    <F_z>=−KT mu0 S [Lcal(A(L))−Lcal(A(0))]
    <a_CM,z>=−KT/L [Lcal(A(L))−Lcal(A(0))]

São identidades exatas dentro dessas hipóteses. Dependem das amplitudes nas duas faces; perfil interno pode alterar respostas locais, sem alterar a integral quando os valores de borda são mantidos.

Pequena amplitude:

    <a_CM,z> ≈ (9/78400)(KT/L)[A(L)²−A(0)²]

Exemplo A²(z)=A0²+beta z, com A²>=0 e A pequeno:

    <F_z> ≈ (9/78400) KT M beta

Amplitudes iguais nas faces zeram a resultante; intercambiá-las inverte seu sinal; mesmas amplitudes de borda, comprimento e KT mantêm a mesma aceleração integrada. Mesma força exige também a mesma massa. Não extrapolar essas identidades a densidade/seção variável, campo autogerado com dinâmica não descrita ou estado transitório.

## 12. Ponte eletrônica–campo e pendências congeladas

Separar: (1) comando elétrico — frequência, fase e duração no ESP32; (2) resposta mensurável — tensão nos piezos, vibração e deformação; (3) amplitude temporal candidata A(z). A ligação de (1)/(2) com (3) ainda não foi estabelecida. Vibração não foi identificada automaticamente como modulação temporal.

Pendências para retomada:
1. Determinar quais registros disponíveis contêm medidas utilizáveis, sem presumir valores não lidos.
2. Formular e justificar a relação sinais/resposta medida → A(z), com unidades e parâmetros explícitos.
3. Determinar ou limitar KT, alpha/M*, ell e v10 por procedimento independente justificável.
4. Examinar autointeração assimétrica e balanço completo de momento e energia.
5. Se houver ensaio autorizado, distinguir configuração simétrica, assimétrica e invertida, com controles e repetibilidade; não tratar isso como alteração já autorizada do protocolo congelado.
6. Manter separadas a extensão material exponencial e a oscilação congelada até definir uma regra explícita de ligação.

## 13. Decisão final

Congelar e preservar esta frente exatamente como hipótese e dedução condicional. Nenhuma previsão numérica de voo, força de bancada, alteração real do tempo ou tempo solar foi estabelecida. Não foram modificados firmware, PCB ou documento canônico anterior. O próximo trabalho começa pelas pendências acima, sem transformar escolhas exploratórias em fundamentos derivados.
