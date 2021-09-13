---
title: Implantar, testar e estender aplicativos migrados
description: 'Descreve como migrar Azure Active Directory (Azure AD) Graph aplicativos para usar a API do Microsoft Graph (REST); isso aborda a etapa 3: implantar, testar e estender.'
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: ec5b9b80ed42e1701619cca9153d7562b663d08f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135974"
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
    O Microsoft Graph oferece suporte a muitos novos conjuntos de dados do Azure Active Directory (Azure AD) e recursos que não estão disponíveis no Azure Active Directory (Azure AD) Graph.

    O Microsoft Graph oferece acesso a muito mais serviços do que apenas Azure Active Directory. É o gateway [da API para Microsoft 365 serviços também.](./index.yml)
    Verifique novos conjuntos de dados e recursos regularmente.  

    - Consulte [Principais serviços e recursos no Microsoft Graph](overview-major-services.md).
    - Confira algumas soluções [de parceiros.](https://developer.microsoft.com/graph/partners)
    - Explore o [blog do Microsoft Graph](https://developer.microsoft.com/graph/blogs) para saber mais sobre o Microsoft Graph e algumas ótimas séries de aprendizado.
    - O [changelog](/graph/changelog) resume atualizações de serviço e documento. Após essas atualizações, você acompanhará novas APIs introduzidas para /beta (visualização) e aquelas promovidas para v1.0 (GA).  Essas novas APIs podem fornecer novas maneiras de adicionar mais valor e novas experiências aos seus aplicativos.  

## <a name="see-also"></a>Confira também

Se você tiver problemas ou precisar de ajuda durante o processo de migração, poderá:

- Revisar a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente
- Postar perguntas para [o Microsoft Graph em Q&A](/answers/topics/microsoft-graph-applications.html) 
- Revise amostras Graph Microsoft para contrastar e comparar com seu código de aplicativo existente:
  - **Aplicativos que usam** a API REST: explorem [inícios rápidos e exemplos,](https://developer.microsoft.com/graph/get-started)escolham sua plataforma de escolha e executem o início rápido ou pesquisem por um exemplo apropriado
  - **App that use the .NET client library**: [review console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>Próximas etapas

- Use [inícios rápidos e exemplos](https://developer.microsoft.com/graph/get-started) para acelerar rapidamente.
- Aproveitar [bibliotecas de clientes e SDKs](/graph/sdks/sdks-overview) para desenvolver aplicativos personalizados 
- Explore os Graph e práticas da [Microsoft.](./overview.md)
- Use [Graph Explorer para](https://aka.ms/ge) experimentar com o Microsoft Graph.
