<!-- markdownlint-disable MD002 MD041 -->

A Conexão de Dados do Microsoft Graph aumenta o modelo transacional do Microsoft Graph com uma maneira inteligente de acessar dados avançados em escala. Os dados abordam como os trabalhadores se comunicam, colaboram e gerenciam seu tempo em todos os aplicativos e serviços no Microsoft 365. Ideal para big data e aprendizado de máquina, A Conexão de Dados permite que você desenvolva aplicativos para análise, inteligência e otimização de processos de negócios, estendendo dados do Microsoft 365 para o Azure. Ao integrar desta forma, você poderá aproveitar o vasto conjunto de computação, armazenamento no Azure, mantendo a conformidade com os padrões do setor e mantendo seus dados seguros.

![Esta imagem explica os controles de dados aplicados entre Microsoft 365 dados na nuvem do Azure, bem como os dados de saída.](images/data-connect-mgdc-capabilities.png)

A Conexão de Dados do Microsoft Graph usa o Azure Data Factory para copiar dados do Microsoft 365 para o armazenamento do seu aplicativo em intervalos configuráveis. Ele também fornece um conjunto de ferramentas para simplificar a entrega desses dados para o Microsoft Azure, permitindo que você acesse as ferramentas de desenvolvimento e hospedagem mais aplicáveis disponíveis. A Conexão de Dados também concede um modelo de controle e consentimento mais granular: você pode gerenciar dados, ver quem está acessando e solicitar propriedades específicas de uma entidade. Isso aprimora o modelo do Microsoft Graph, que concede ou nega acesso a aplicativos a entidades inteiras.

Você pode usar o data Conexão para habilitar cenários de aprendizado de máquina para sua organização.. Nesses cenários, você pode criar aplicações que forneçam informações valiosas aos seus participantes, treinar modelos de aprendizado de máquina e até mesmo realizar previsões com base em grandes quantidades de dados adquiridos.

## <a name="get-started"></a>Introdução

Neste tutorial, você criará seu primeiro aplicativo de Conexão de Dados do Microsoft Graph. Interessante, não é? Também acreditamos nisso! Para começar, você precisará configurar algumas coisas primeiro.

### <a name="prerequisites"></a>Pré-requisitos

Para concluir esse laboratório, você precisará das seguintes assinaturas ou licenças.

1. **Microsoft 365 deenancy**
  
   - Se você não tiver um, você obterá um (gratuitamente) ao se inscrever no programa Microsoft 365 [Desenvolvedor.](https://developer.microsoft.com/microsoft-365/dev-program)
   - Vários Microsoft 365 usuários com emails enviados e recebidos.
   - Acesso a pelo menos duas contas que atendem aos seguintes requisitos:
      - Deve ter a **função de administrador global** atribuída.
      - Deve ter acesso à Central Administração Microsoft 365.

1. **Assinatura do Microsoft Azure**
  
   - Se você não tiver um, poderá obter um (gratuitamente) em nosso [site do Azure.](https://azure.microsoft.com/free/)
   - A conta usada para entrar deve ter a função de administrador **global** concedida a ela.
   - A assinatura do Azure deve estar no mesmo locatário que o locatário Microsoft 365, pois o Graph Data Conexão exportará apenas dados para uma assinatura do Azure no mesmo locatário, não entre locatários.
   - Seus Microsoft 365 e locatários do Azure devem estar no mesmo Microsoft Azure Active Directory locatário.

1. Certifique-se de que [você Visual Studio](https://visualstudio.microsoft.com/vs/) instalado em sua máquina de desenvolvimento.

> [!NOTE]
> As capturas de tela e os exemplos usados neste laboratório são de um locatário de Microsoft 365 de teste com exemplo de email de usuários de teste. Você pode usar seu próprio Microsoft 365 locatário para executar as mesmas etapas. Nenhum dado é gravado em Microsoft 365. Uma cópia dos dados de email é extraída de todos os usuários em um locatário do Microsoft 365 e copiada para uma conta do Azure Blob Armazenamento que você mantém o controle sobre quem tem acesso aos dados no Azure Blob Armazenamento.
