---
title: tipo de recurso appIdentity
description: Indica a identidade do aplicativo que executou a ação ou foi alterada. Inclui ID do aplicativo, nome, ID da entidade de serviço e nome. Este recurso é chamado pela API directoryAudit
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dc2f6f912eafdacfc05eb11b65140995dfa28cec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532116"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="466bf-105">tipo de recurso appIdentity</span><span class="sxs-lookup"><span data-stu-id="466bf-105">appIdentity resource type</span></span>

<span data-ttu-id="466bf-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="466bf-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="466bf-107">Indica a identidade do aplicativo que executou a ação ou foi alterada.</span><span class="sxs-lookup"><span data-stu-id="466bf-107">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="466bf-108">Inclui a ID de aplicativo, o nome e a ID e o nome da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="466bf-108">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="466bf-109">Este recurso é usado pela operação [Get directoryAudit](../api/directoryaudit-get.md) .</span><span class="sxs-lookup"><span data-stu-id="466bf-109">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="466bf-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="466bf-110">Properties</span></span>

| <span data-ttu-id="466bf-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="466bf-111">Property</span></span>     | <span data-ttu-id="466bf-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="466bf-112">Type</span></span>   |<span data-ttu-id="466bf-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="466bf-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="466bf-114">appId</span><span class="sxs-lookup"><span data-stu-id="466bf-114">appId</span></span>|<span data-ttu-id="466bf-115">String</span><span class="sxs-lookup"><span data-stu-id="466bf-115">String</span></span>|<span data-ttu-id="466bf-116">Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="466bf-116">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="466bf-117">displayName</span><span class="sxs-lookup"><span data-stu-id="466bf-117">displayName</span></span>|<span data-ttu-id="466bf-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="466bf-118">String</span></span>|<span data-ttu-id="466bf-119">Refere-se ao nome do aplicativo exibido no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="466bf-119">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="466bf-120">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="466bf-120">servicePrincipalId</span></span>|<span data-ttu-id="466bf-121">String</span><span class="sxs-lookup"><span data-stu-id="466bf-121">String</span></span>|<span data-ttu-id="466bf-122">Refere-se ao GUID exclusivo indicando a ID da entidade de serviço no Azure Active Directory para o aplicativo correspondente.</span><span class="sxs-lookup"><span data-stu-id="466bf-122">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="466bf-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="466bf-123">servicePrincipalName</span></span>|<span data-ttu-id="466bf-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="466bf-124">String</span></span>|<span data-ttu-id="466bf-125">Refere-se ao nome da entidade de segurança do serviço é o nome do aplicativo no locatário.</span><span class="sxs-lookup"><span data-stu-id="466bf-125">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="466bf-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="466bf-126">JSON representation</span></span>

<span data-ttu-id="466bf-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="466bf-127">Here is a JSON representation of the resource.</span></span>

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
