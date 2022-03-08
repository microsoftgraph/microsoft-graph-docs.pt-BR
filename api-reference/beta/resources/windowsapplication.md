---
title: Tipo de recurso windowsApplication
description: Representa configurações para aplicativos que executam o Microsoft Windows e publicados no Microsoft Store ou no armazenamento de jogos do Xbox.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: aricrowe57
ms.openlocfilehash: 7caedf0d8f8cda38129cfc108a2e4dc7ce609279
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338023"
---
# <a name="webapplication-resource-type"></a>Tipo de recurso webApplication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações para aplicativos que executam o Microsoft Windows e publicados no Microsoft Store ou no armazenamento de jogos do Xbox.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| packageSid | Cadeia de caracteres | O identificador de segurança do pacote que a Microsoft atribuiu ao aplicativo. Opcional. Somente leitura. |
| redirectUris | String collection | Especifica as URLs para as quais os tokens de usuário são enviados para entrada ou urIs de redirecionamento para as quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados. Disponível apenas para aplicativos que suportam `PersonalMicrosoftAccount` **o signInAudience**. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.windowsApplication"
}-->

```json
{
  "packageSid": "String",
  "redirectUris": ["String"]
}

```