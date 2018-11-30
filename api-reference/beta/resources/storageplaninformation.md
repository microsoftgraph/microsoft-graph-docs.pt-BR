---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
ms.openlocfilehash: 07552f405ec8c5d6ae8345a8238cd8aec3763b11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038147"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="3eb83-102">tipo de recurso de storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="3eb83-102">storagePlanInformation resource type</span></span>

> <span data-ttu-id="3eb83-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3eb83-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eb83-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3eb83-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3eb83-105">O recurso de **storagePlanInformation** fornece informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="3eb83-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="3eb83-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3eb83-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```
## <a name="properties"></a><span data-ttu-id="3eb83-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3eb83-107">Properties</span></span>

| <span data-ttu-id="3eb83-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3eb83-108">Property name</span></span>     | <span data-ttu-id="3eb83-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3eb83-109">Type</span></span>      | <span data-ttu-id="3eb83-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eb83-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="3eb83-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="3eb83-111">upgradeAvailable</span></span>  | <span data-ttu-id="3eb83-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb83-112">Boolean</span></span>   | <span data-ttu-id="3eb83-113">Indica se os planos de cota de armazenamento mais estarão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="3eb83-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="3eb83-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eb83-114">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

