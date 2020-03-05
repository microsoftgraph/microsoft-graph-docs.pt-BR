---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c7f832fdce72f2490a45b3dae206eb7de28c686
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448022"
---
# <a name="organization-resource-type"></a><span data-ttu-id="e6c83-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="e6c83-103">organization resource type</span></span>

<span data-ttu-id="e6c83-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e6c83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6c83-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6c83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6c83-106">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="e6c83-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="e6c83-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6c83-107">Methods</span></span>
|<span data-ttu-id="e6c83-108">Método</span><span class="sxs-lookup"><span data-stu-id="e6c83-108">Method</span></span>|<span data-ttu-id="e6c83-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6c83-109">Return Type</span></span>|<span data-ttu-id="e6c83-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6c83-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6c83-111">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="e6c83-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="e6c83-112">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="e6c83-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="e6c83-113">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e6c83-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="e6c83-114">Obter organização</span><span class="sxs-lookup"><span data-stu-id="e6c83-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="e6c83-115">organization</span><span class="sxs-lookup"><span data-stu-id="e6c83-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e6c83-116">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e6c83-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e6c83-117">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="e6c83-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="e6c83-118">organização</span><span class="sxs-lookup"><span data-stu-id="e6c83-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e6c83-119">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e6c83-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e6c83-120">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e6c83-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="e6c83-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c83-121">Int32</span></span>|<span data-ttu-id="e6c83-122">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="e6c83-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="e6c83-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6c83-123">Properties</span></span>
|<span data-ttu-id="e6c83-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6c83-124">Property</span></span>|<span data-ttu-id="e6c83-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6c83-125">Type</span></span>|<span data-ttu-id="e6c83-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6c83-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6c83-127">id</span><span class="sxs-lookup"><span data-stu-id="e6c83-127">id</span></span>|<span data-ttu-id="e6c83-128">String</span><span class="sxs-lookup"><span data-stu-id="e6c83-128">String</span></span>|<span data-ttu-id="e6c83-129">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="e6c83-129">The GUID for the object.</span></span>|
|<span data-ttu-id="e6c83-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e6c83-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e6c83-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="e6c83-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="e6c83-132">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="e6c83-132">Mobile device management authority.</span></span> <span data-ttu-id="e6c83-133">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="e6c83-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6c83-134">Relações</span><span class="sxs-lookup"><span data-stu-id="e6c83-134">Relationships</span></span>
<span data-ttu-id="e6c83-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6c83-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6c83-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6c83-136">JSON Representation</span></span>
<span data-ttu-id="e6c83-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6c83-137">Here is a JSON representation of the resource.</span></span>
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




