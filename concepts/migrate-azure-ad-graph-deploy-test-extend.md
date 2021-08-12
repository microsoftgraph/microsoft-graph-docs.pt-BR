---
title: Implantar, testar e estender aplicativos migrados
description: 'Descreve como migrar aplicativos Azure Active Directory (Azure AD) para usar a API do Microsoft Graph (REST); isso aborda a etapa 3: implantar, testar e estender.'
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: c950e8fe97fd6a7e5a269824b1745af08b256c6795bbebb9186f105550233e1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163526"
---
# <a name="deploy-test-and-extend"></a>Implantar, testar e estender

Esta é a etapa 4 do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

1.  **Testar corretamente**

    Depois de atualizar seu aplicativo, teste-o completamente para verificar se ele funciona conforme o esperado e se você não introduziu nenhuma regressão.  

    Use vários ambientes, conjuntos de dados e personas de usuário final, por exemplo, credenciais com funções, direitos e responsabilidades diferentes. Vá por todo o ciclo de vida, fazendo com que um novo usuário de teste adquira o aplicativo pela primeira vez, bem como um usuário existente (que já consentiu) tentando usar o aplicativo novamente.

2.  **Implantar atualizações em estágios**

    Considere implantar suas atualizações em estágios.  Uma rolagem limitada para um pequeno conjunto de usuários amigáveis pode ajudar a identificar falhas e outros problemas potencialmente embaraçosos.  Isso também oferece a você a chance de monitorar a recepção inicial e os comentários.

    Se a implantação inicial der certo, monitore o progresso à medida que você implanta em audiências maiores.

3.  **Explorar novo valor**

    Agora que você alternou para o Microsoft Graph, nunca foi mais fácil desbloquear muitos mais conjuntos de dados e recursos que agora estão à sua ponta dos dedos. 
    O Microsoft Graph oferece suporte a muitos novos conjuntos de dados e recursos do Azure AD que não estão disponíveis no Azure AD Graph, incluindo: 

    - [Microsoft 365 gerenciamento de grupo](./office365-groups-concept-overview.md)
    - [Convites de usuário externos](/graph/api/resources/invitation)
    - A capacidade de [restaurar usuários e Microsoft 365 grupos depois](/graph/api/resources/directory) que eles foram excluídos
    - [Notificações de webhook em usuários e grupos](./webhooks.md?toc=.%252fref%252ftoc.json)
    - Recursos de governança de identidade, como:
      - [PiM](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) (gerenciamento de identidade privilegiada) para elevar os usuários a funções privilegiadas somente quando necessário e por um período de tempo limitado
      - [Avaliações do Access](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) para análises de acesso única ou recorrentes para atestado dos direitos de acesso do usuário
      - [Termos de uso para permitir que](/graph/api/resources/agreement) as organizações apresentem informações para requisitos legais ou de conformidade, como avisos de isenção de responsabilidade
    - Recursos de segurança como:
      - [Eventos de risco de identidade](/graph/api/resources/riskdetection)
      - [Usuários de risco](/graph/api/resources/riskyuser)
    - [Bibliotecas de clientes e exemplos](/graph/sdks/sdks-overview) disponíveis em muitas outras plataformas e idiomas. Os SDKs do Microsoft Graph fornecem uma interface descobrivel para acessar facilmente seus dados enquanto manipulam de forma transparente a aquisição de tokens, a manipulação de novo devido a erros e a throttling, tratamento seguro de redirecionamento e serialização de modelo e dessarialização.

    O Microsoft Graph oferece acesso a muito mais serviços do que apenas Azure Active Directory. É o gateway [da API para Microsoft 365 serviços também.](./index.yml)
    Verifique novos conjuntos de dados e recursos regularmente.  

    - Confira algumas soluções [de parceiros.](https://developer.microsoft.com/graph/partners)
    - Explore o [blog do Microsoft Graph](https://developer.microsoft.com/graph/blogs) para saber mais sobre o Microsoft Graph e algumas ótimas séries de aprendizado.
    - O [changelog](/graph/changelog) resume atualizações de serviço e documento. Após essas atualizações, você acompanhará novas APIs introduzidas para /beta (visualização) e aquelas promovidas para v1.0 (GA).  Essas novas APIs podem fornecer novas maneiras de adicionar mais valor e novas experiências aos seus aplicativos.  

## <a name="see-also"></a>Confira também

Se você tiver problemas ou precisar de ajuda durante o processo de migração, poderá:

- Revisar a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente
- Postar perguntas para [o Microsoft Q&A](/answers/topics/microsoft-graph-applications.html) 
- Revise amostras Graph Microsoft para contrastar e comparar com seu código de aplicativo existente:
  - **Aplicativos que usam** a API REST : explorar [inícios rápidos e exemplos,](https://developer.microsoft.com/graph/get-started)escolher sua plataforma de escolha e executar o início rápido ou pesquisar por um exemplo apropriado
  - **App that use the .NET client library**: [review console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>Próximos passos

- Use [inícios rápidos e exemplos](https://developer.microsoft.com/graph/get-started) para acelerar rapidamente.
- Aproveitar [bibliotecas de clientes e SDKs](/graph/sdks/sdks-overview) para desenvolver aplicativos personalizados 
- Explore os Graph e práticas da [Microsoft.](./overview.md)
- Use [Graph Explorer para](https://aka.ms/ge) experimentar com o Microsoft Graph.