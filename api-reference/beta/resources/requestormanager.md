---
title: Tipo complexo requestorManager
description: Identifica uma relação com outro usuário no locatário que será permitido como aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4bfd42854a55ec2daa9e380c539a25479b0e933
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761076"
---
# <a name="requestormanager-complex-type"></a><span data-ttu-id="8efa1-103">Tipo complexo requestorManager</span><span class="sxs-lookup"><span data-stu-id="8efa1-103">requestorManager complex type</span></span>

<span data-ttu-id="8efa1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8efa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8efa1-105">Usado nas configurações de aprovação de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8efa1-105">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="8efa1-106">É um subtipo de [userSet](userset.md), no qual o valor indica que o gerente de um usuário solicitante `@odata.type` deve ser o `#microsoft.graph.requestorManager` aprovador.</span><span class="sxs-lookup"><span data-stu-id="8efa1-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="8efa1-107">Ao criar um estágio de aprovação da política de atribuição de pacote de acesso com requestorManager, inclua também outro aprovador, como um único usuário ou membro do grupo, caso o usuário solicitante não tenha um gerente.</span><span class="sxs-lookup"><span data-stu-id="8efa1-107">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="8efa1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8efa1-108">Properties</span></span>


| <span data-ttu-id="8efa1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8efa1-109">Property</span></span>                     | <span data-ttu-id="8efa1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8efa1-110">Type</span></span>                      | <span data-ttu-id="8efa1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8efa1-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="8efa1-112">isBackup</span><span class="sxs-lookup"><span data-stu-id="8efa1-112">isBackup</span></span> | <span data-ttu-id="8efa1-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8efa1-113">Boolean</span></span> | <span data-ttu-id="8efa1-114">Para um gerente em um estágio de aprovação, indica se o gerente é um aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="8efa1-114">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |
|<span data-ttu-id="8efa1-115">managerLevel</span><span class="sxs-lookup"><span data-stu-id="8efa1-115">managerLevel</span></span> | <span data-ttu-id="8efa1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8efa1-116">Int32</span></span> | <span data-ttu-id="8efa1-117">O nível hierárquico do gerente em relação ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="8efa1-117">The hierarchical level of the manager with respect to the requestor.</span></span> <span data-ttu-id="8efa1-118">Por exemplo, o gerente direto de um solicitante teria um managerLevel de 1, enquanto o gerente do gerente do solicitante teria um managerLevel de 2.</span><span class="sxs-lookup"><span data-stu-id="8efa1-118">For example, the direct manager of a requestor would have a managerLevel of 1, while the manager of the requestor's manager would have a managerLevel of 2.</span></span> <span data-ttu-id="8efa1-119">O valor padrão para managerLevel é 1.</span><span class="sxs-lookup"><span data-stu-id="8efa1-119">Default value for managerLevel is 1.</span></span> <span data-ttu-id="8efa1-120">Os valores possíveis para essa propriedade variam de 1 a 2.</span><span class="sxs-lookup"><span data-stu-id="8efa1-120">Possible values for this property range from 1 to 2.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="8efa1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8efa1-121">JSON representation</span></span>

<span data-ttu-id="8efa1-122">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="8efa1-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "managerLevel": 1
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


