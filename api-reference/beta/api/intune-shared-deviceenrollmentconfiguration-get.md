---
title: Obter deviceEnrollmentConfiguration
description: Ler propriedades e relações do objeto deviceEnrollmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6925e91ff6d1974ea0073de92724020196b98597
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864204"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="da334-103">Obter deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="da334-103">Get deviceEnrollmentConfiguration</span></span>

<span data-ttu-id="da334-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da334-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da334-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da334-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da334-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da334-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da334-107">Ler propriedades e relações do objeto [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da334-107">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da334-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da334-108">Prerequisites</span></span>
<span data-ttu-id="da334-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da334-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da334-111">Permission type</span></span>|<span data-ttu-id="da334-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da334-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da334-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da334-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="da334-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="da334-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="da334-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="da334-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="da334-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="da334-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="da334-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="da334-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="da334-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da334-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da334-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da334-119">Not supported.</span></span>|
|<span data-ttu-id="da334-120">Application</span><span class="sxs-lookup"><span data-stu-id="da334-120">Application</span></span>||
| <span data-ttu-id="da334-121">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="da334-121">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="da334-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="da334-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="da334-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="da334-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="da334-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="da334-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da334-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da334-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da334-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da334-126">Optional query parameters</span></span>
<span data-ttu-id="da334-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da334-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da334-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da334-128">Request headers</span></span>
|<span data-ttu-id="da334-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da334-129">Header</span></span>|<span data-ttu-id="da334-130">Valor</span><span class="sxs-lookup"><span data-stu-id="da334-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da334-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="da334-131">Authorization</span></span>|<span data-ttu-id="da334-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da334-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da334-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da334-133">Accept</span></span>|<span data-ttu-id="da334-134">application/json</span><span class="sxs-lookup"><span data-stu-id="da334-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da334-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da334-135">Request body</span></span>
<span data-ttu-id="da334-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da334-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da334-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="da334-137">Response</span></span>
<span data-ttu-id="da334-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da334-138">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da334-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da334-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="da334-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da334-140">Request</span></span>
<span data-ttu-id="da334-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da334-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="da334-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="da334-142">Response</span></span>
<span data-ttu-id="da334-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da334-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
    "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7
  }
}
```







