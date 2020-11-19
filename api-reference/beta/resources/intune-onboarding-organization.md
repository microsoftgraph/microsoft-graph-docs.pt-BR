---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30dbbb5b7a86b39acceabc2ebf8df74caafca9c9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259540"
---
# <a name="organization-resource-type"></a><span data-ttu-id="a0cab-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="a0cab-103">organization resource type</span></span>

<span data-ttu-id="a0cab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0cab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0cab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0cab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0cab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0cab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0cab-107">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="a0cab-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="a0cab-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a0cab-108">Methods</span></span>
|<span data-ttu-id="a0cab-109">Método</span><span class="sxs-lookup"><span data-stu-id="a0cab-109">Method</span></span>|<span data-ttu-id="a0cab-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a0cab-110">Return Type</span></span>|<span data-ttu-id="a0cab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0cab-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a0cab-112">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="a0cab-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="a0cab-113">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="a0cab-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="a0cab-114">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="a0cab-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="a0cab-115">Obter organização</span><span class="sxs-lookup"><span data-stu-id="a0cab-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="a0cab-116">organization</span><span class="sxs-lookup"><span data-stu-id="a0cab-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="a0cab-117">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="a0cab-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="a0cab-118">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="a0cab-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="a0cab-119">organização</span><span class="sxs-lookup"><span data-stu-id="a0cab-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="a0cab-120">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="a0cab-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="a0cab-121">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="a0cab-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="a0cab-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a0cab-122">Int32</span></span>|<span data-ttu-id="a0cab-123">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="a0cab-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="a0cab-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0cab-124">Properties</span></span>
|<span data-ttu-id="a0cab-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0cab-125">Property</span></span>|<span data-ttu-id="a0cab-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0cab-126">Type</span></span>|<span data-ttu-id="a0cab-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0cab-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0cab-128">id</span><span class="sxs-lookup"><span data-stu-id="a0cab-128">id</span></span>|<span data-ttu-id="a0cab-129">String</span><span class="sxs-lookup"><span data-stu-id="a0cab-129">String</span></span>|<span data-ttu-id="a0cab-130">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="a0cab-130">The GUID for the object.</span></span>|
|<span data-ttu-id="a0cab-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="a0cab-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="a0cab-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="a0cab-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="a0cab-133">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="a0cab-133">Mobile device management authority.</span></span> <span data-ttu-id="a0cab-134">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="a0cab-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="a0cab-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="a0cab-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="a0cab-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="a0cab-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="a0cab-137">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="a0cab-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0cab-138">Relações</span><span class="sxs-lookup"><span data-stu-id="a0cab-138">Relationships</span></span>
<span data-ttu-id="a0cab-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0cab-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0cab-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0cab-140">JSON Representation</span></span>
<span data-ttu-id="a0cab-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0cab-141">Here is a JSON representation of the resource.</span></span>
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




