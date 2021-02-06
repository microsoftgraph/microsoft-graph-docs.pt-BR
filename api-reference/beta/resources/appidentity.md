---
title: Tipo de recurso appIdentity
description: Indica a identidade do aplicativo que realizou a ação ou foi alterado. Inclui id do aplicativo, nome, ID da entidade de serviço e nome. Esse recurso é chamado pela API directoryAudit
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: sureshja
ms.openlocfilehash: 2949acd00b3ef494d7fb3999c180631cf8609cc3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137043"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="a2811-105">Tipo de recurso appIdentity</span><span class="sxs-lookup"><span data-stu-id="a2811-105">appIdentity resource type</span></span>

<span data-ttu-id="a2811-106">Namespace: microsoft.graph Indica a identidade do aplicativo que realizou a ação ou foi alterado.</span><span class="sxs-lookup"><span data-stu-id="a2811-106">Namespace: microsoft.graph Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="a2811-107">Inclui id do aplicativo, nome, ID da entidade de serviço e nome.</span><span class="sxs-lookup"><span data-stu-id="a2811-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="a2811-108">Esse recurso é chamado pela API [directoryAudit](../api/directoryaudit-get.md)</span><span class="sxs-lookup"><span data-stu-id="a2811-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="a2811-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2811-109">Properties</span></span>
| <span data-ttu-id="a2811-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2811-110">Property</span></span>     | <span data-ttu-id="a2811-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2811-111">Type</span></span>   |<span data-ttu-id="a2811-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2811-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2811-113">appId</span><span class="sxs-lookup"><span data-stu-id="a2811-113">appId</span></span>|<span data-ttu-id="a2811-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2811-114">String</span></span>|<span data-ttu-id="a2811-115">Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a2811-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="a2811-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a2811-116">displayName</span></span>|<span data-ttu-id="a2811-117">String</span><span class="sxs-lookup"><span data-stu-id="a2811-117">String</span></span>|<span data-ttu-id="a2811-118">Refere-se ao Nome do Aplicativo exibido no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a2811-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="a2811-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="a2811-119">servicePrincipalId</span></span>|<span data-ttu-id="a2811-120">String</span><span class="sxs-lookup"><span data-stu-id="a2811-120">String</span></span>|<span data-ttu-id="a2811-121">Refere-se ao GUID exclusivo que indica a ID da entidade de serviço no Azure Active Directory para o aplicativo correspondente.</span><span class="sxs-lookup"><span data-stu-id="a2811-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="a2811-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2811-122">servicePrincipalName</span></span>|<span data-ttu-id="a2811-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2811-123">String</span></span>|<span data-ttu-id="a2811-124">Refere-se ao nome da entidade de serviço é o nome do aplicativo no locatário.</span><span class="sxs-lookup"><span data-stu-id="a2811-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2811-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2811-125">JSON representation</span></span>

<span data-ttu-id="a2811-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2811-126">Here is a JSON representation of the resource.</span></span>

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


