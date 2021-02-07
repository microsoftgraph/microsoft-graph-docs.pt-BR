---
title: Tipo de recurso appIdentity
description: Indica a identidade do aplicativo que realizou a ação ou foi alterado. Inclui id do aplicativo, nome, ID da entidade de serviço e nome. Esse recurso é chamado pela API directoryAudit
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d0ba66e962f70a854fd028305b1e31c140ad1fe8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134992"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="9a150-105">Tipo de recurso appIdentity</span><span class="sxs-lookup"><span data-stu-id="9a150-105">appIdentity resource type</span></span>

<span data-ttu-id="9a150-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a150-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a150-107">Indica a identidade do aplicativo que realizou a ação ou foi alterado.</span><span class="sxs-lookup"><span data-stu-id="9a150-107">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="9a150-108">Inclui a ID do aplicativo, o nome e a ID da entidade de serviço e o nome.</span><span class="sxs-lookup"><span data-stu-id="9a150-108">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="9a150-109">Esse recurso é usado pela [operação Get directoryAudit.](../api/directoryaudit-get.md)</span><span class="sxs-lookup"><span data-stu-id="9a150-109">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="9a150-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a150-110">Properties</span></span>

| <span data-ttu-id="9a150-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a150-111">Property</span></span>     | <span data-ttu-id="9a150-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a150-112">Type</span></span>   |<span data-ttu-id="9a150-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a150-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a150-114">appId</span><span class="sxs-lookup"><span data-stu-id="9a150-114">appId</span></span>|<span data-ttu-id="9a150-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a150-115">String</span></span>|<span data-ttu-id="9a150-116">Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9a150-116">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="9a150-117">displayName</span><span class="sxs-lookup"><span data-stu-id="9a150-117">displayName</span></span>|<span data-ttu-id="9a150-118">String</span><span class="sxs-lookup"><span data-stu-id="9a150-118">String</span></span>|<span data-ttu-id="9a150-119">Refere-se ao Nome do Aplicativo exibido no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9a150-119">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="9a150-120">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="9a150-120">servicePrincipalId</span></span>|<span data-ttu-id="9a150-121">String</span><span class="sxs-lookup"><span data-stu-id="9a150-121">String</span></span>|<span data-ttu-id="9a150-122">Refere-se ao GUID exclusivo que indica a ID da entidade de serviço no Azure Active Directory para o aplicativo correspondente.</span><span class="sxs-lookup"><span data-stu-id="9a150-122">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="9a150-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a150-123">servicePrincipalName</span></span>|<span data-ttu-id="9a150-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a150-124">String</span></span>|<span data-ttu-id="9a150-125">Refere-se ao nome da entidade de serviço é o nome do aplicativo no locatário.</span><span class="sxs-lookup"><span data-stu-id="9a150-125">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a150-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a150-126">JSON representation</span></span>

<span data-ttu-id="9a150-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a150-127">Here is a JSON representation of the resource.</span></span>

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

