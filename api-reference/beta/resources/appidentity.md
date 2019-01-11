---
title: tipo de recurso de appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui o Id do aplicativo, nome, ID de entidade de serviço e Name. Este recurso é chamado pelo API directoryAudit
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855780"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="56215-105">tipo de recurso de appIdentity</span><span class="sxs-lookup"><span data-stu-id="56215-105">appIdentity resource type</span></span>
<span data-ttu-id="56215-106">Indica a identidade do aplicativo que executou a ação ou foi alterada.</span><span class="sxs-lookup"><span data-stu-id="56215-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="56215-107">Inclui o Id do aplicativo, nome, ID de entidade de serviço e Name.</span><span class="sxs-lookup"><span data-stu-id="56215-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="56215-108">Este recurso é chamado pelo [directoryAudit](../api/directoryaudit-get.md) API</span><span class="sxs-lookup"><span data-stu-id="56215-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="56215-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56215-109">Properties</span></span>
| <span data-ttu-id="56215-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56215-110">Property</span></span>     | <span data-ttu-id="56215-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="56215-111">Type</span></span>   |<span data-ttu-id="56215-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="56215-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56215-113">appId</span><span class="sxs-lookup"><span data-stu-id="56215-113">appId</span></span>|<span data-ttu-id="56215-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56215-114">String</span></span>|<span data-ttu-id="56215-115">Refere-se o GUID exclusivo que representa a Id do aplicativo no Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="56215-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="56215-116">displayName</span><span class="sxs-lookup"><span data-stu-id="56215-116">displayName</span></span>|<span data-ttu-id="56215-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56215-117">String</span></span>|<span data-ttu-id="56215-118">Refere-se ao nome do aplicativo exibido no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="56215-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="56215-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="56215-119">servicePrincipalId</span></span>|<span data-ttu-id="56215-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56215-120">String</span></span>|<span data-ttu-id="56215-121">Refere-se o GUID exclusivo que indica o Id da entidade de serviço no Windows Azure Active Directory para o aplicativo correspondente.</span><span class="sxs-lookup"><span data-stu-id="56215-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="56215-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="56215-122">servicePrincipalName</span></span>|<span data-ttu-id="56215-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56215-123">String</span></span>|<span data-ttu-id="56215-124">Refere-se para o nome de entidade de serviço é o nome do aplicativo no inquilino.</span><span class="sxs-lookup"><span data-stu-id="56215-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56215-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56215-125">JSON representation</span></span>

<span data-ttu-id="56215-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56215-126">Here is a JSON representation of the resource.</span></span>

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
