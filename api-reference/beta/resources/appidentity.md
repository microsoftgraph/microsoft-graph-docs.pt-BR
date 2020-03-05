---
title: tipo de recurso appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui ID do aplicativo, nome, ID da entidade de serviço e nome. Este recurso é chamado pela API directoryAudit
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 08cb797f56d26b4b421fb25210f7dad2715c70d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508300"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="3a9d8-105">tipo de recurso appIdentity</span><span class="sxs-lookup"><span data-stu-id="3a9d8-105">appIdentity resource type</span></span>

<span data-ttu-id="3a9d8-106">Namespace: Microsoft. Graph indica a identidade do aplicativo que executou a ação ou foi alterada.</span><span class="sxs-lookup"><span data-stu-id="3a9d8-106">Namespace: microsoft.graph Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="3a9d8-107">Inclui ID do aplicativo, nome, ID da entidade de serviço e nome.</span><span class="sxs-lookup"><span data-stu-id="3a9d8-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="3a9d8-108">Este recurso é chamado pela API [directoryAudit](../api/directoryaudit-get.md)</span><span class="sxs-lookup"><span data-stu-id="3a9d8-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="3a9d8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a9d8-109">Properties</span></span>
| <span data-ttu-id="3a9d8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a9d8-110">Property</span></span>     | <span data-ttu-id="3a9d8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a9d8-111">Type</span></span>   |<span data-ttu-id="3a9d8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a9d8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a9d8-113">appId</span><span class="sxs-lookup"><span data-stu-id="3a9d8-113">appId</span></span>|<span data-ttu-id="3a9d8-114">String</span><span class="sxs-lookup"><span data-stu-id="3a9d8-114">String</span></span>|<span data-ttu-id="3a9d8-115">Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3a9d8-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="3a9d8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="3a9d8-116">displayName</span></span>|<span data-ttu-id="3a9d8-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a9d8-117">String</span></span>|<span data-ttu-id="3a9d8-118">Refere-se ao nome do aplicativo exibido no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3a9d8-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="3a9d8-119">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a9d8-119">servicePrincipalId</span></span>|<span data-ttu-id="3a9d8-120">String</span><span class="sxs-lookup"><span data-stu-id="3a9d8-120">String</span></span>|<span data-ttu-id="3a9d8-121">Refere-se ao GUID exclusivo indicando a ID da entidade de serviço no Azure Active Directory para o aplicativo correspondente.</span><span class="sxs-lookup"><span data-stu-id="3a9d8-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="3a9d8-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a9d8-122">servicePrincipalName</span></span>|<span data-ttu-id="3a9d8-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a9d8-123">String</span></span>|<span data-ttu-id="3a9d8-124">Refere-se ao nome da entidade de segurança do serviço é o nome do aplicativo no locatário.</span><span class="sxs-lookup"><span data-stu-id="3a9d8-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3a9d8-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a9d8-125">JSON representation</span></span>

<span data-ttu-id="3a9d8-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a9d8-126">Here is a JSON representation of the resource.</span></span>

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
