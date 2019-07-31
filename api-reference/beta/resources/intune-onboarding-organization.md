---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76ef47ee4db5d7858ac476fd12db1615180bd18b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998013"
---
# <a name="organization-resource-type"></a><span data-ttu-id="ba2b3-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="ba2b3-103">organization resource type</span></span>

> <span data-ttu-id="ba2b3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba2b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba2b3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba2b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba2b3-106">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="ba2b3-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="ba2b3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ba2b3-107">Methods</span></span>
|<span data-ttu-id="ba2b3-108">Método</span><span class="sxs-lookup"><span data-stu-id="ba2b3-108">Method</span></span>|<span data-ttu-id="ba2b3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ba2b3-109">Return Type</span></span>|<span data-ttu-id="ba2b3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba2b3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba2b3-111">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="ba2b3-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="ba2b3-112">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="ba2b3-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="ba2b3-113">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ba2b3-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="ba2b3-114">Obter organização</span><span class="sxs-lookup"><span data-stu-id="ba2b3-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="ba2b3-115">organization</span><span class="sxs-lookup"><span data-stu-id="ba2b3-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ba2b3-116">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ba2b3-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ba2b3-117">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="ba2b3-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="ba2b3-118">organização</span><span class="sxs-lookup"><span data-stu-id="ba2b3-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ba2b3-119">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="ba2b3-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ba2b3-120">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ba2b3-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="ba2b3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ba2b3-121">Int32</span></span>|<span data-ttu-id="ba2b3-122">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="ba2b3-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="ba2b3-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba2b3-123">Properties</span></span>
|<span data-ttu-id="ba2b3-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba2b3-124">Property</span></span>|<span data-ttu-id="ba2b3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba2b3-125">Type</span></span>|<span data-ttu-id="ba2b3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba2b3-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba2b3-127">id</span><span class="sxs-lookup"><span data-stu-id="ba2b3-127">id</span></span>|<span data-ttu-id="ba2b3-128">String</span><span class="sxs-lookup"><span data-stu-id="ba2b3-128">String</span></span>|<span data-ttu-id="ba2b3-129">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ba2b3-129">The GUID for the object.</span></span>|
|<span data-ttu-id="ba2b3-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ba2b3-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="ba2b3-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="ba2b3-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="ba2b3-132">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="ba2b3-132">Mobile device management authority.</span></span> <span data-ttu-id="ba2b3-133">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="ba2b3-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="ba2b3-134">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="ba2b3-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="ba2b3-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="ba2b3-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="ba2b3-136">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="ba2b3-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba2b3-137">Relações</span><span class="sxs-lookup"><span data-stu-id="ba2b3-137">Relationships</span></span>
<span data-ttu-id="ba2b3-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba2b3-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba2b3-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba2b3-139">JSON Representation</span></span>
<span data-ttu-id="ba2b3-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba2b3-140">Here is a JSON representation of the resource.</span></span>
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
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```





