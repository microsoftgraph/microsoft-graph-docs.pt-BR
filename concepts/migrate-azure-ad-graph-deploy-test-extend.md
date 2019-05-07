---
title: Implantar, testar e estender aplicativos migrados
description: 'Descreve como migrar aplicativos do Azure Active Directory (Azure AD) para usar a API do Microsoft Graph (REST); isso aborda a etapa 3: implantar, testar e estender.'
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8a63c14ef27648a1d586551ebe12e18a5f263a9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630248"
---
# <a name="deploy-test-and-extend"></a>Implantar, testar e estender

Esta é a etapa 4 do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

1.  **Teste por meio**

    Depois de atualizar o aplicativo, teste-o cuidadosamente para verificar se ele funciona conforme o esperado e se você não introduziu nenhuma regressão.  

    Certifique-se de usar vários ambientes, conjuntos de dados e pessoas de usuário final, por exemplo, credenciais com diferentes funções, direitos e responsabilidades. Percorra todo o ciclo de vida, fazendo com que um novo usuário de teste adquira o aplicativo pela primeira vez, bem como um usuário existente (que já tenha remetido) tentando usar o aplicativo novamente.

2.  **Implantar atualizações em estágios**

    Considere a implantação de suas atualizações em estágios.  Uma distribuição limitada para um pequeno conjunto de usuários amigáveis pode ajudar a identificar falhas e outros problemas desagradáveis.  Isso também lhe dá a oportunidade de monitorar a recepção inicial e os comentários.

    Se a distribuição inicial ficar bem, monitore o progresso à medida que você implanta em grandes audiências.

3.  **Explorar novo valor**

    Agora você já fez a migração para o Microsoft Graph, nunca foi mais fácil desbloquear muito mais conjuntos de informações e recursos que agora estão em suas mãos. Verifique se há novos conjuntos de recursos e capacidades regularmente.  

    - Dê uma olhada no [que você pode fazer com o Microsoft Graph](/graph/examples)
    - Explore o [blog do Microsoft Graph](/graph/blogs) para obter as últimas notícias sobre o Microsoft Graph e algumas boas séries de aprendizado.
    - O [changelog](/greaph/changelog) resume as atualizações de serviço e de documento. Seguir essas atualizações o ajudará a rastrear novas APIs introduzidas no/beta (visualização) e aquelas promovidas para a versão v 1.0 (GA).  Essas novas APIs podem fornecer novas maneiras de adicionar mais valor e novas experiências aos seus aplicativos.  

## <a name="see-also"></a>Confira também

Se você encontrar problemas ou precisar de ajuda durante o processo de migração, você pode:

- Revise a [lista de verificação](migrate-azure-ad-graph-overview.md) novamente
- Postar perguntas no [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)
- Revise as amostras do Microsoft Graph para comparar e comparar com o código do aplicativo existente:
  - **Aplicativos que usam a API REST**: explorar [inícios e amostras rápidas](/graph/get-started), escolhendo sua plataforma de escolha e executar o início rápido ou pesquisar um exemplo apropriado
  - **Aplicativo que usa a biblioteca de cliente .net**: examinar [console-Csharp-Snippets-Sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) e/ou [dotnetcore-console-Sample](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>Próximos passos

- Use [inícios e amostras rápidas](/graph/get-started) para se familiarizar rapidamente.
- Aproveitar [bibliotecas de clientes e SDKs](https://developer.microsoft.com/graph/get-started) para desenvolver aplicativos personalizados 
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
