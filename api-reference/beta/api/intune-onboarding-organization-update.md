---
title: Atualize a organização
description: Atualizar as propriedades de um objeto organização.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0c6771f1fb879f3b233b6315bbd2fe379d8f74b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352424"
---
# <a name="update-organization"></a><span data-ttu-id="811ee-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="811ee-103">Update organization</span></span>

> <span data-ttu-id="811ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="811ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="811ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="811ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="811ee-106">Atualizar as propriedades de um objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="811ee-106">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="811ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="811ee-107">Prerequisites</span></span>
<span data-ttu-id="811ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="811ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="811ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="811ee-110">Permission type</span></span>|<span data-ttu-id="811ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="811ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="811ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="811ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="811ee-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="811ee-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="811ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="811ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="811ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="811ee-115">Not supported.</span></span>|
|<span data-ttu-id="811ee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="811ee-116">Application</span></span>|<span data-ttu-id="811ee-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="811ee-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="811ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="811ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="811ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="811ee-119">Request headers</span></span>
|<span data-ttu-id="811ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="811ee-120">Header</span></span>|<span data-ttu-id="811ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="811ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="811ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="811ee-122">Authorization</span></span>|<span data-ttu-id="811ee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="811ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="811ee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="811ee-124">Accept</span></span>|<span data-ttu-id="811ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="811ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="811ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="811ee-126">Request body</span></span>
<span data-ttu-id="811ee-127">No corpo da solicitação, forneça uma representação JSON do objeto [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="811ee-127">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="811ee-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="811ee-128">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="811ee-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="811ee-129">Property</span></span>|<span data-ttu-id="811ee-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="811ee-130">Type</span></span>|<span data-ttu-id="811ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="811ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="811ee-132">id</span><span class="sxs-lookup"><span data-stu-id="811ee-132">id</span></span>|<span data-ttu-id="811ee-133">String</span><span class="sxs-lookup"><span data-stu-id="811ee-133">String</span></span>|<span data-ttu-id="811ee-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="811ee-134">The GUID for the object.</span></span>|
|<span data-ttu-id="811ee-135">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="811ee-135">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="811ee-136">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="811ee-136">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="811ee-137">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="811ee-137">Mobile device management authority.</span></span> <span data-ttu-id="811ee-138">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="811ee-138">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="811ee-139">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="811ee-139">certificateConnectorSetting</span></span>|[<span data-ttu-id="811ee-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="811ee-140">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="811ee-141">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="811ee-141">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="811ee-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="811ee-142">Response</span></span>
<span data-ttu-id="811ee-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="811ee-143">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="811ee-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="811ee-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="811ee-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="811ee-145">Request</span></span>
<span data-ttu-id="811ee-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="811ee-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 492

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```

### <a name="response"></a><span data-ttu-id="811ee-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="811ee-147">Response</span></span>
<span data-ttu-id="811ee-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="811ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```






