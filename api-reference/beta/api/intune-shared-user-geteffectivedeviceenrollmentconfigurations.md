---
title: função getEffectiveDeviceEnrollmentConfigurations
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee8eb2ff3a15d234d05ed28a13f600e7e47e4d53
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527137"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="d26f6-103">função getEffectiveDeviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="d26f6-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="d26f6-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d26f6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d26f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d26f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d26f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d26f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d26f6-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d26f6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d26f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d26f6-108">Prerequisites</span></span>

<span data-ttu-id="d26f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d26f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d26f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d26f6-111">Permission type</span></span>|<span data-ttu-id="d26f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d26f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d26f6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d26f6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d26f6-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="d26f6-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d26f6-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d26f6-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d26f6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d26f6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d26f6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d26f6-117">Not supported.</span></span>|
|<span data-ttu-id="d26f6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d26f6-118">Application</span></span>|<span data-ttu-id="d26f6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d26f6-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d26f6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d26f6-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d26f6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d26f6-121">Request headers</span></span>

|<span data-ttu-id="d26f6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d26f6-122">Header</span></span>|<span data-ttu-id="d26f6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d26f6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d26f6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d26f6-124">Authorization</span></span>|<span data-ttu-id="d26f6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d26f6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d26f6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d26f6-126">Accept</span></span>|<span data-ttu-id="d26f6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d26f6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d26f6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d26f6-128">Request body</span></span>

<span data-ttu-id="d26f6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d26f6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d26f6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d26f6-130">Response</span></span>

<span data-ttu-id="d26f6-131">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d26f6-131">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d26f6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d26f6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d26f6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d26f6-133">Request</span></span>

<span data-ttu-id="d26f6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d26f6-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="d26f6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d26f6-135">Response</span></span>

<span data-ttu-id="d26f6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d26f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



