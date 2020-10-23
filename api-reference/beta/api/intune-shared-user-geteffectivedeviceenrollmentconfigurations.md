---
title: função getEffectiveDeviceEnrollmentConfigurations
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b613834d06427f1687b839a79c2c24f14630c82
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728617"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="5054d-103">função getEffectiveDeviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="5054d-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

<span data-ttu-id="5054d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5054d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5054d-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5054d-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5054d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5054d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5054d-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5054d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5054d-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5054d-108">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5054d-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5054d-109">Prerequisites</span></span>

<span data-ttu-id="5054d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5054d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5054d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5054d-112">Permission type</span></span>|<span data-ttu-id="5054d-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5054d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5054d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5054d-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5054d-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="5054d-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5054d-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5054d-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5054d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5054d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5054d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5054d-118">Not supported.</span></span>|
|<span data-ttu-id="5054d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5054d-119">Application</span></span>||
| <span data-ttu-id="5054d-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="5054d-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5054d-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5054d-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="5054d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5054d-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5054d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5054d-123">Request headers</span></span>

|<span data-ttu-id="5054d-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5054d-124">Header</span></span>|<span data-ttu-id="5054d-125">Valor</span><span class="sxs-lookup"><span data-stu-id="5054d-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5054d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5054d-126">Authorization</span></span>|<span data-ttu-id="5054d-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5054d-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5054d-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5054d-128">Accept</span></span>|<span data-ttu-id="5054d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5054d-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5054d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5054d-130">Request body</span></span>

<span data-ttu-id="5054d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5054d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5054d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5054d-132">Response</span></span>

<span data-ttu-id="5054d-133">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5054d-133">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5054d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5054d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="5054d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5054d-135">Request</span></span>

<span data-ttu-id="5054d-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5054d-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="5054d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5054d-137">Response</span></span>

<span data-ttu-id="5054d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5054d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











