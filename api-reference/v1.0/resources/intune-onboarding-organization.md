---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2e4fffa10e81ba83a28fd6eebfc3ba4bf870d7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441739"
---
# <a name="organization-resource-type"></a><span data-ttu-id="fc052-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="fc052-103">organization resource type</span></span>

<span data-ttu-id="fc052-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc052-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc052-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc052-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc052-106">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="fc052-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="fc052-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc052-107">Methods</span></span>
|<span data-ttu-id="fc052-108">Método</span><span class="sxs-lookup"><span data-stu-id="fc052-108">Method</span></span>|<span data-ttu-id="fc052-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc052-109">Return Type</span></span>|<span data-ttu-id="fc052-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc052-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fc052-111">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="fc052-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="fc052-112">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="fc052-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="fc052-113">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="fc052-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="fc052-114">Obter organização</span><span class="sxs-lookup"><span data-stu-id="fc052-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="fc052-115">organization</span><span class="sxs-lookup"><span data-stu-id="fc052-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="fc052-116">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="fc052-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="fc052-117">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="fc052-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="fc052-118">organização</span><span class="sxs-lookup"><span data-stu-id="fc052-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="fc052-119">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="fc052-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="fc052-120">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="fc052-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="fc052-121">Int32</span><span class="sxs-lookup"><span data-stu-id="fc052-121">Int32</span></span>|<span data-ttu-id="fc052-122">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="fc052-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="fc052-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc052-123">Properties</span></span>
|<span data-ttu-id="fc052-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc052-124">Property</span></span>|<span data-ttu-id="fc052-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc052-125">Type</span></span>|<span data-ttu-id="fc052-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc052-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc052-127">id</span><span class="sxs-lookup"><span data-stu-id="fc052-127">id</span></span>|<span data-ttu-id="fc052-128">String</span><span class="sxs-lookup"><span data-stu-id="fc052-128">String</span></span>|<span data-ttu-id="fc052-129">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="fc052-129">The GUID for the object.</span></span>|
|<span data-ttu-id="fc052-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="fc052-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="fc052-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="fc052-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="fc052-132">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="fc052-132">Mobile device management authority.</span></span> <span data-ttu-id="fc052-133">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="fc052-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc052-134">Relações</span><span class="sxs-lookup"><span data-stu-id="fc052-134">Relationships</span></span>
<span data-ttu-id="fc052-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc052-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc052-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc052-136">JSON Representation</span></span>
<span data-ttu-id="fc052-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc052-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->







