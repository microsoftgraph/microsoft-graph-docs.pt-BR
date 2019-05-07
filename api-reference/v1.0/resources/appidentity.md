---
title: tipo de recurso appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui ID do aplicativo, nome, ID da entidade de serviço e nome. Este recurso é chamado pela API directoryAudit
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a4e7f5a21d5140537e745f7234186ad3b24098f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629352"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="fadbf-105">tipo de recurso appIdentity</span><span class="sxs-lookup"><span data-stu-id="fadbf-105">appIdentity resource type</span></span>

<span data-ttu-id="fadbf-106">Indica a identidade do aplicativo que executou a ação ou foi alterada.</span><span class="sxs-lookup"><span data-stu-id="fadbf-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="fadbf-107">Inclui a ID de aplicativo, o nome e a ID e o nome da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="fadbf-107">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="fadbf-108">Este recurso é usado pela operação [Get directoryAudit](../api/directoryaudit-get.md) .</span><span class="sxs-lookup"><span data-stu-id="fadbf-108">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="fadbf-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fadbf-109">Properties</span></span>

| <span data-ttu-id="fadbf-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fadbf-110">Property</span></span>     | <span data-ttu-id="fadbf-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fadbf-111">Type</span></span>   |<span data-ttu-id="fadbf-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fadbf-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fadbf-113">appId</span><span class="sxs-lookup"><span data-stu-id="fadbf-113">appId</span></span>|<span data-ttu-id="fadbf-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fadbf-114">String</span></span>|<span data-ttu-id="fadbf-115">Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fadbf-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="fadbf-116">displayName</span><span class="sxs-lookup"><span data-stu-id="fadbf-116">displayName</span></span>|<span data-ttu-id="fadbf-117">String</span><span class="sxs-lookup"><span data-stu-id="fadbf-117">String</span></span>|<span data-ttu-id="fadbf-118">Refere-se ao nome do aplicativo exibido no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fadbf-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="fadbf-119">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="fadbf-119">servicePrincipalId</span></span>|<span data-ttu-id="fadbf-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fadbf-120">String</span></span>|<span data-ttu-id="fadbf-121">Refere-se ao GUID exclusivo indicando a ID da entidade de serviço no Azure Active Directory para o aplicativo correspondente.</span><span class="sxs-lookup"><span data-stu-id="fadbf-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="fadbf-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="fadbf-122">servicePrincipalName</span></span>|<span data-ttu-id="fadbf-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fadbf-123">String</span></span>|<span data-ttu-id="fadbf-124">Refere-se ao nome da entidade de segurança do serviço é o nome do aplicativo no locatário.</span><span class="sxs-lookup"><span data-stu-id="fadbf-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fadbf-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fadbf-125">JSON representation</span></span>

<span data-ttu-id="fadbf-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fadbf-126">Here is a JSON representation of the resource.</span></span>

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
