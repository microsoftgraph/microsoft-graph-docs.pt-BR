---
title: função getEffectiveDeviceEnrollmentConfigurations
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28c0f774192f3fde33c654047d10f67ad7cffdcd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725848"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="b6b48-103">função getEffectiveDeviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="b6b48-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="b6b48-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6b48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6b48-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6b48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6b48-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6b48-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6b48-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6b48-107">Prerequisites</span></span>
<span data-ttu-id="b6b48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6b48-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6b48-110">Permission type</span></span>|<span data-ttu-id="b6b48-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6b48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6b48-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6b48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6b48-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6b48-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b6b48-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6b48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6b48-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6b48-115">Not supported.</span></span>|
|<span data-ttu-id="b6b48-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6b48-116">Application</span></span>|<span data-ttu-id="b6b48-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6b48-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6b48-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6b48-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b6b48-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b48-119">Request headers</span></span>
|<span data-ttu-id="b6b48-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6b48-120">Header</span></span>|<span data-ttu-id="b6b48-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b6b48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6b48-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6b48-122">Authorization</span></span>|<span data-ttu-id="b6b48-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6b48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6b48-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6b48-124">Accept</span></span>|<span data-ttu-id="b6b48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6b48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6b48-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b48-126">Request body</span></span>
<span data-ttu-id="b6b48-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6b48-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6b48-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6b48-128">Response</span></span>
<span data-ttu-id="b6b48-129">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6b48-129">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6b48-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6b48-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6b48-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b48-131">Request</span></span>
<span data-ttu-id="b6b48-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6b48-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="b6b48-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6b48-133">Response</span></span>
<span data-ttu-id="b6b48-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6b48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```





