---
title: Examinar o uso do aplicativo APIs do Azure AD Graph
description: Descreve como auditar as APIs do Azure Active Directory (Azure AD) para migrar um aplicativo para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ecf6d1897d8473b42ac8b5bcb45c59747eb36f13
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630269"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>Examinar o uso do aplicativo APIs do Azure AD Graph

Esta é a etapa 2 do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Ao planejar sua migração para o Microsoft Graph, Reserve um tempo para revisar seu aplicativo existente e catalogar as APIs do Azure AD Graph que você está usando no momento.

Compare sua lista com as diferenças conhecidas.  Isso ajuda a identificar alterações específicas que você precisará fazer para migrar seu aplicativo.  Eles incluem alterações simples facilmente resolvidas usando os recursos de pesquisa e substituição de um editor ou atualizações mais complicadas que podem exigir mais análise.

O Microsoft Graph oferece suporte a muitos dos mesmos recursos e funcionalidades do Azure AD Graph.  Há algumas diferenças importantes:

- [Solicitar diferenças](migrate-azure-ad-graph-request-differences.md)
- [Diferenças de recursos](migrate-azure-ad-graph-feature-differences.md)
- [Diferenças de tipo de recurso](migrate-azure-ad-graph-resource-differences.md)
- [Diferenças de propriedade](migrate-azure-ad-graph-property-differences.md)
- [Diferenças de método](migrate-azure-ad-graph-method-differences.md)

Você também deve verificar as permissões necessárias para os recursos que seu aplicativo está usando.  Em alguns casos, as permissões mais granulares estão disponíveis.

Para saber mais, confira [permissões](/concepts/permissions-reference.md).

## <a name="next-steps"></a>Próximos passos

- Saiba mais sobre [as diferenças de registro de aplicativo, permissões e consentimento](migrate-azure-ad-graph-app-registration.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
