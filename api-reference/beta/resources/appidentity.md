---
title: tipo de recurso de appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui o Id do aplicativo, nome, ID de entidade de serviço e Name. Este recurso é chamado pelo API directoryAudit
ms.openlocfilehash: 6fcbe8dbb1e17139111c5f1fa9e8681cd1b996a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036960"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="743ed-105">tipo de recurso de appIdentity</span><span class="sxs-lookup"><span data-stu-id="743ed-105">appIdentity resource type</span></span>
<span data-ttu-id="743ed-106">Indica a identidade do aplicativo que executou a ação ou foi alterada.</span><span class="sxs-lookup"><span data-stu-id="743ed-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="743ed-107">Inclui o Id do aplicativo, nome, ID de entidade de serviço e Name.</span><span class="sxs-lookup"><span data-stu-id="743ed-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="743ed-108">Este recurso é chamado pelo [directoryAudit](../api/directoryaudit-get.md) API</span><span class="sxs-lookup"><span data-stu-id="743ed-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="743ed-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="743ed-109">Properties</span></span>
| <span data-ttu-id="743ed-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="743ed-110">Property</span></span>     | <span data-ttu-id="743ed-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="743ed-111">Type</span></span>   |<span data-ttu-id="743ed-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="743ed-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="743ed-113">appId</span><span class="sxs-lookup"><span data-stu-id="743ed-113">appId</span></span>|<span data-ttu-id="743ed-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="743ed-114">String</span></span>|<span data-ttu-id="743ed-115">Refere-se o GUID exclusivo que representa a Id do aplicativo no Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="743ed-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="743ed-116">displayName</span><span class="sxs-lookup"><span data-stu-id="743ed-116">displayName</span></span>|<span data-ttu-id="743ed-117">String</span><span class="sxs-lookup"><span data-stu-id="743ed-117">String</span></span>|<span data-ttu-id="743ed-118">Refere-se ao nome do aplicativo exibido no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="743ed-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="743ed-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="743ed-119">servicePrincipalId</span></span>|<span data-ttu-id="743ed-120">String</span><span class="sxs-lookup"><span data-stu-id="743ed-120">String</span></span>|<span data-ttu-id="743ed-121">Refere-se o GUID exclusivo que indica o Id da entidade de serviço no Windows Azure Active Directory para o aplicativo correspondente.</span><span class="sxs-lookup"><span data-stu-id="743ed-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="743ed-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="743ed-122">servicePrincipalName</span></span>|<span data-ttu-id="743ed-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="743ed-123">String</span></span>|<span data-ttu-id="743ed-124">Refere-se para o nome de entidade de serviço é o nome do aplicativo no inquilino.</span><span class="sxs-lookup"><span data-stu-id="743ed-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="743ed-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="743ed-125">JSON representation</span></span>

<span data-ttu-id="743ed-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="743ed-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->