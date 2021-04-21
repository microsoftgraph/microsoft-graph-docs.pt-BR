---
title: Implantar, testar e estender aplicativos migrados
description: 'Descreve como migrar aplicativos do Azure Active Directory (Azure AD) para usar a API do Microsoft Graph (REST); isso aborda a etapa 3: implantar, testar e estender.'
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: cdd2414652e675223b6de42a6a63de5c7e8c5c8a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921921"
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
    O Microsoft Graph dá suporte a muitos novos conjuntos de dados e recursos do Azure AD que não estão disponíveis no Azure AD Graph, incluindo: 

    - [Gerenciamento de grupo do Microsoft 365](./office365-groups-concept-overview.md)
    - [Convites de usuário externos](/graph/api/resources/invitation?view=graph-rest-1.0)
    - A capacidade de restaurar usuários e grupos do [Microsoft 365](/graph/api/resources/directory?view=graph-rest-1.0) depois que eles foram excluídos
    - [Notificações de webhook em usuários e grupos](./webhooks.md?toc=.%252fref%252ftoc.json&view=graph-rest-1.0)
    - Recursos de governança de identidade, como:
      - [PiM](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (gerenciamento de identidade privilegiada) para elevar os usuários a funções privilegiadas somente quando necessário e por um período de tempo limitado
      - [Avaliações do Access](/graph/api/resources/accessreviews-root?view=graph-rest-beta) para análises de acesso única ou recorrentes para atestado dos direitos de acesso do usuário
      - [Termos de uso para permitir que](/graph/api/resources/accessreviews-root?view=graph-rest-beta) as organizações apresentem informações para requisitos legais ou de conformidade, como avisos de isenção de responsabilidade
    - Recursos de segurança como:
      - [Eventos de risco de identidade](/graph/api/resources/identityriskevent?view=graph-rest-1.0)
      - [Usuários de risco](/graph/api/resources/riskyuser?view=graph-rest-1.0)
    - [Bibliotecas de clientes e exemplos](./index.yml) disponíveis em muitas outras plataformas e idiomas. Os SDKs do Microsoft Graph fornecem uma interface descobrivel para acessar facilmente seus dados enquanto manipulam de forma transparente a aquisição de tokens, a manipulação de novo devido a erros e a throttling, manipulação segura de redirecionamento e serialização de modelo e dessarialização.

    O Microsoft Graph oferece acesso a muito mais serviços do que apenas ao Azure Active Directory. Também é o gateway da API para serviços do [Microsoft 365.](./index.yml)
    Verifique novos conjuntos de dados e recursos regularmente.  

    - Dê uma olhada [no que você pode fazer com o Microsoft Graph](/graph/examples)
    - Explore o [blog do Microsoft Graph](/graph/blogs) para saber mais sobre o Microsoft Graph e algumas ótimas séries de aprendizado.
    - O [changelog](/greaph/changelog) resume atualizações de serviço e documento. Após essas atualizações, você acompanhará novas APIs introduzidas para /beta (visualização) e aquelas promovidas para v1.0 (GA).  Essas novas APIs podem fornecer novas maneiras de adicionar mais valor e novas experiências aos seus aplicativos.  

## <a name="see-also"></a>Confira também

Se você tiver problemas ou precisar de ajuda durante o processo de migração, poderá:

- Revisar a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente
- Postar perguntas para [o Microsoft Q&A](/answers/topics/microsoft-graph-applications.html) 
- Revise exemplos do Microsoft Graph para contrastar e comparar com seu código de aplicativo existente:
  - **Aplicativos que usam** a API REST : explorar [inícios rápidos e exemplos,](https://developer.microsoft.com/graph/get-started)escolher sua plataforma de escolha e executar o início rápido ou pesquisar por um exemplo apropriado
  - **App that use the .NET client library**: [review console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>Próximas Etapas

- Use [inícios rápidos e exemplos](/graph/get-started) para acelerar rapidamente.
- Aproveitar [bibliotecas de clientes e SDKs](https://developer.microsoft.com/graph/get-started) para desenvolver aplicativos personalizados 
- Explore conceitos e práticas do [Microsoft Graph.](./overview.md)
- Use [o Graph Explorer](https://aka.ms/ge) para experimentar com o Microsoft Graph.