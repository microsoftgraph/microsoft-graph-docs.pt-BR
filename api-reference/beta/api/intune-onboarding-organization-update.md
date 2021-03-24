---
title: Atualize a organização
description: Atualizar as propriedades de um objeto organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f110c15c81661a3c4b12ccc137cc8b6abfcc8c7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148747"
---
# <a name="update-organization"></a><span data-ttu-id="f43dc-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="f43dc-103">Update organization</span></span>

<span data-ttu-id="f43dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f43dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f43dc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f43dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f43dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f43dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f43dc-107">Atualizar as propriedades de um objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f43dc-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f43dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f43dc-108">Prerequisites</span></span>
<span data-ttu-id="f43dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f43dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f43dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f43dc-111">Permission type</span></span>|<span data-ttu-id="f43dc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f43dc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f43dc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f43dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f43dc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f43dc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f43dc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f43dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f43dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f43dc-116">Not supported.</span></span>|
|<span data-ttu-id="f43dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f43dc-117">Application</span></span>|<span data-ttu-id="f43dc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f43dc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f43dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f43dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="f43dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f43dc-120">Request headers</span></span>
|<span data-ttu-id="f43dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f43dc-121">Header</span></span>|<span data-ttu-id="f43dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f43dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f43dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f43dc-123">Authorization</span></span>|<span data-ttu-id="f43dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f43dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f43dc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f43dc-125">Accept</span></span>|<span data-ttu-id="f43dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f43dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f43dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f43dc-127">Request body</span></span>
<span data-ttu-id="f43dc-128">No corpo da solicitação, forneça uma representação JSON do objeto [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f43dc-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="f43dc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f43dc-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="f43dc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f43dc-130">Property</span></span>|<span data-ttu-id="f43dc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f43dc-131">Type</span></span>|<span data-ttu-id="f43dc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f43dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f43dc-133">id</span><span class="sxs-lookup"><span data-stu-id="f43dc-133">id</span></span>|<span data-ttu-id="f43dc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f43dc-134">String</span></span>|<span data-ttu-id="f43dc-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="f43dc-135">The GUID for the object.</span></span>|
|<span data-ttu-id="f43dc-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="f43dc-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="f43dc-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="f43dc-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="f43dc-138">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="f43dc-138">Mobile device management authority.</span></span> <span data-ttu-id="f43dc-139">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="f43dc-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="f43dc-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f43dc-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="f43dc-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f43dc-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="f43dc-142">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="f43dc-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="f43dc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f43dc-143">Response</span></span>
<span data-ttu-id="f43dc-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f43dc-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f43dc-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f43dc-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="f43dc-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f43dc-146">Request</span></span>
<span data-ttu-id="f43dc-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f43dc-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f43dc-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f43dc-148">Response</span></span>
<span data-ttu-id="f43dc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f43dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




