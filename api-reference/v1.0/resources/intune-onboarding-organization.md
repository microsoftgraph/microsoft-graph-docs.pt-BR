---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2af65c341f665fd358d03619a3cd3606723df123
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754948"
---
# <a name="organization-resource-type"></a><span data-ttu-id="cc6fb-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="cc6fb-103">organization resource type</span></span>

<span data-ttu-id="cc6fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc6fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc6fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc6fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc6fb-106">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="cc6fb-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="cc6fb-107">Methods</span><span class="sxs-lookup"><span data-stu-id="cc6fb-107">Methods</span></span>
|<span data-ttu-id="cc6fb-108">Método</span><span class="sxs-lookup"><span data-stu-id="cc6fb-108">Method</span></span>|<span data-ttu-id="cc6fb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc6fb-109">Return Type</span></span>|<span data-ttu-id="cc6fb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc6fb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc6fb-111">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="cc6fb-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="cc6fb-112">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="cc6fb-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="cc6fb-113">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="cc6fb-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="cc6fb-114">Obter organização</span><span class="sxs-lookup"><span data-stu-id="cc6fb-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="cc6fb-115">organization</span><span class="sxs-lookup"><span data-stu-id="cc6fb-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="cc6fb-116">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="cc6fb-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="cc6fb-117">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="cc6fb-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="cc6fb-118">organização</span><span class="sxs-lookup"><span data-stu-id="cc6fb-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="cc6fb-119">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="cc6fb-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="cc6fb-120">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="cc6fb-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="cc6fb-121">Int32</span><span class="sxs-lookup"><span data-stu-id="cc6fb-121">Int32</span></span>|<span data-ttu-id="cc6fb-122">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="cc6fb-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="cc6fb-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc6fb-123">Properties</span></span>
|<span data-ttu-id="cc6fb-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc6fb-124">Property</span></span>|<span data-ttu-id="cc6fb-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc6fb-125">Type</span></span>|<span data-ttu-id="cc6fb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc6fb-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc6fb-127">id</span><span class="sxs-lookup"><span data-stu-id="cc6fb-127">id</span></span>|<span data-ttu-id="cc6fb-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc6fb-128">String</span></span>|<span data-ttu-id="cc6fb-129">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="cc6fb-129">The GUID for the object.</span></span>|
|<span data-ttu-id="cc6fb-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="cc6fb-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="cc6fb-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="cc6fb-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="cc6fb-132">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="cc6fb-132">Mobile device management authority.</span></span> <span data-ttu-id="cc6fb-133">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="cc6fb-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc6fb-134">Relações</span><span class="sxs-lookup"><span data-stu-id="cc6fb-134">Relationships</span></span>
<span data-ttu-id="cc6fb-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cc6fb-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc6fb-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc6fb-136">JSON Representation</span></span>
<span data-ttu-id="cc6fb-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc6fb-137">Here is a JSON representation of the resource.</span></span>
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




