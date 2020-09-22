---
title: Listar macOSGeneralDeviceConfigurations
description: Listar propriedades e relações dos objetos macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afcd5de61dbebf648995499e76f9b5de2d551158
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028907"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="81ff8-103">Listar macOSGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="81ff8-103">List macOSGeneralDeviceConfigurations</span></span>

<span data-ttu-id="81ff8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81ff8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81ff8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81ff8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81ff8-106">Listar propriedades e relações dos objetos [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81ff8-106">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81ff8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81ff8-107">Prerequisites</span></span>
<span data-ttu-id="81ff8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81ff8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81ff8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81ff8-110">Permission type</span></span>|<span data-ttu-id="81ff8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81ff8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81ff8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81ff8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81ff8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81ff8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="81ff8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81ff8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81ff8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81ff8-115">Not supported.</span></span>|
|<span data-ttu-id="81ff8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81ff8-116">Application</span></span>|<span data-ttu-id="81ff8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81ff8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81ff8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81ff8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="81ff8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81ff8-119">Request headers</span></span>
|<span data-ttu-id="81ff8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81ff8-120">Header</span></span>|<span data-ttu-id="81ff8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81ff8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81ff8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81ff8-122">Authorization</span></span>|<span data-ttu-id="81ff8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81ff8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81ff8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81ff8-124">Accept</span></span>|<span data-ttu-id="81ff8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81ff8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ff8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81ff8-126">Request body</span></span>
<span data-ttu-id="81ff8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81ff8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81ff8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ff8-128">Response</span></span>
<span data-ttu-id="81ff8-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81ff8-129">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81ff8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81ff8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="81ff8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81ff8-131">Request</span></span>
<span data-ttu-id="81ff8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81ff8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="81ff8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ff8-133">Response</span></span>
<span data-ttu-id="81ff8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81ff8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
      "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "emailInDomainSuffixes": [
        "Email In Domain Suffixes value"
      ],
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumCharacterSetCount": 0,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true
    }
  ]
}
```









