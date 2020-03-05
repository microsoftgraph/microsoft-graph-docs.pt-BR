---
title: tipo complexo requestorManager
description: Identifica uma relação com outro usuário no locatário que será permitido como Aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b2e3062383dd1cc1c7d04342b2dcbd5be0afd67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521121"
---
# <a name="requestomanager-complex-type"></a><span data-ttu-id="dc4f4-103">tipo complexo requestoManager</span><span class="sxs-lookup"><span data-stu-id="dc4f4-103">requestoManager complex type</span></span>

<span data-ttu-id="dc4f4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dc4f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc4f4-105">Usado nas configurações de aprovação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc4f4-105">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="dc4f4-106">É um subtipo de [userset](userset.md), no qual o `@odata.type` valor `#microsoft.graph.requestorManager` indica que o gerente de um usuário solicitante é o aprovador.</span><span class="sxs-lookup"><span data-stu-id="dc4f4-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="dc4f4-107">Ao criar um estágio de aprovação de política de atribuição de pacote do Access com o requestorManager, também inclua outro aprovador, como um único usuário ou membro de grupo, caso o usuário solicitante não tenha um gerente.</span><span class="sxs-lookup"><span data-stu-id="dc4f4-107">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="dc4f4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc4f4-108">Properties</span></span>


| <span data-ttu-id="dc4f4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc4f4-109">Property</span></span>                     | <span data-ttu-id="dc4f4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc4f4-110">Type</span></span>                      | <span data-ttu-id="dc4f4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc4f4-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="dc4f4-112">IsBackup</span><span class="sxs-lookup"><span data-stu-id="dc4f4-112">isBackup</span></span> | <span data-ttu-id="dc4f4-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc4f4-113">Boolean</span></span> | <span data-ttu-id="dc4f4-114">Para um gerente em um estágio de aprovação, indica se o gerente é um Aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="dc4f4-114">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dc4f4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc4f4-115">JSON representation</span></span>

<span data-ttu-id="dc4f4-116">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="dc4f4-116">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
