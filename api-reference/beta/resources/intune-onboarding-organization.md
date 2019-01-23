---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b47ec69063998a935640f05d04a17bfc5714c8d8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398230"
---
# <a name="organization-resource-type"></a><span data-ttu-id="abfd3-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="abfd3-103">organization resource type</span></span>

> <span data-ttu-id="abfd3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="abfd3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="abfd3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="abfd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abfd3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="abfd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abfd3-107">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="abfd3-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="abfd3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="abfd3-108">Methods</span></span>
|<span data-ttu-id="abfd3-109">Método</span><span class="sxs-lookup"><span data-stu-id="abfd3-109">Method</span></span>|<span data-ttu-id="abfd3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="abfd3-110">Return Type</span></span>|<span data-ttu-id="abfd3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="abfd3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="abfd3-112">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="abfd3-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="abfd3-113">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="abfd3-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="abfd3-114">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="abfd3-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="abfd3-115">Obter organização</span><span class="sxs-lookup"><span data-stu-id="abfd3-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="abfd3-116">organização</span><span class="sxs-lookup"><span data-stu-id="abfd3-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="abfd3-117">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="abfd3-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="abfd3-118">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="abfd3-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="abfd3-119">organização</span><span class="sxs-lookup"><span data-stu-id="abfd3-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="abfd3-120">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="abfd3-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="abfd3-121">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="abfd3-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="abfd3-122">Int32</span><span class="sxs-lookup"><span data-stu-id="abfd3-122">Int32</span></span>|<span data-ttu-id="abfd3-123">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="abfd3-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="abfd3-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abfd3-124">Properties</span></span>
|<span data-ttu-id="abfd3-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abfd3-125">Property</span></span>|<span data-ttu-id="abfd3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="abfd3-126">Type</span></span>|<span data-ttu-id="abfd3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="abfd3-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abfd3-128">id</span><span class="sxs-lookup"><span data-stu-id="abfd3-128">id</span></span>|<span data-ttu-id="abfd3-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abfd3-129">String</span></span>|<span data-ttu-id="abfd3-130">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="abfd3-130">The GUID for the object.</span></span>|
|<span data-ttu-id="abfd3-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="abfd3-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="abfd3-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="abfd3-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="abfd3-133">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="abfd3-133">Mobile device management authority.</span></span> <span data-ttu-id="abfd3-134">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="abfd3-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="abfd3-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="abfd3-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="abfd3-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="abfd3-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="abfd3-137">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="abfd3-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abfd3-138">Relações</span><span class="sxs-lookup"><span data-stu-id="abfd3-138">Relationships</span></span>
<span data-ttu-id="abfd3-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="abfd3-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="abfd3-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abfd3-140">JSON Representation</span></span>
<span data-ttu-id="abfd3-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abfd3-141">Here is a JSON representation of the resource.</span></span>
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




