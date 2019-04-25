---
title: tipo de recurso appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui ID do aplicativo, nome, ID da entidade de serviço e nome. Este recurso é chamado pela API directoryAudit
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535673"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="f8a8b-105">tipo de recurso appIdentity</span><span class="sxs-lookup"><span data-stu-id="f8a8b-105">appIdentity resource type</span></span>
<span data-ttu-id="f8a8b-106">Indica a identidade do aplicativo que executou a ação ou foi alterada.</span><span class="sxs-lookup"><span data-stu-id="f8a8b-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="f8a8b-107">Inclui ID do aplicativo, nome, ID da entidade de serviço e nome.</span><span class="sxs-lookup"><span data-stu-id="f8a8b-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="f8a8b-108">Este recurso é chamado pela API [directoryAudit](../api/directoryaudit-get.md)</span><span class="sxs-lookup"><span data-stu-id="f8a8b-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="f8a8b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8a8b-109">Properties</span></span>
| <span data-ttu-id="f8a8b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8a8b-110">Property</span></span>     | <span data-ttu-id="f8a8b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8a8b-111">Type</span></span>   |<span data-ttu-id="f8a8b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8a8b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8a8b-113">appId</span><span class="sxs-lookup"><span data-stu-id="f8a8b-113">appId</span></span>|<span data-ttu-id="f8a8b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8a8b-114">String</span></span>|<span data-ttu-id="f8a8b-115">Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8a8b-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="f8a8b-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f8a8b-116">displayName</span></span>|<span data-ttu-id="f8a8b-117">String</span><span class="sxs-lookup"><span data-stu-id="f8a8b-117">String</span></span>|<span data-ttu-id="f8a8b-118">Refere-se ao nome do aplicativo exibido no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8a8b-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="f8a8b-119">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8a8b-119">servicePrincipalId</span></span>|<span data-ttu-id="f8a8b-120">String</span><span class="sxs-lookup"><span data-stu-id="f8a8b-120">String</span></span>|<span data-ttu-id="f8a8b-121">Refere-se ao GUID exclusivo indicando a ID da entidade de serviço no Azure Active Directory para o aplicativo correspondente.</span><span class="sxs-lookup"><span data-stu-id="f8a8b-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="f8a8b-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8a8b-122">servicePrincipalName</span></span>|<span data-ttu-id="f8a8b-123">String</span><span class="sxs-lookup"><span data-stu-id="f8a8b-123">String</span></span>|<span data-ttu-id="f8a8b-124">Refere-se ao nome da entidade de segurança do serviço é o nome do aplicativo no locatário.</span><span class="sxs-lookup"><span data-stu-id="f8a8b-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f8a8b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8a8b-125">JSON representation</span></span>

<span data-ttu-id="f8a8b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8a8b-126">Here is a JSON representation of the resource.</span></span>

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
