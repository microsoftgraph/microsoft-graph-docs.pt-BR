---
title: Listar macOSGeneralDeviceConfigurations
description: Listar propriedades e relações dos objetos macOSGeneralDeviceConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 955094df6493b8c6224e9b41d0032d5971bb22f3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514302"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="2bc1c-103">Listar macOSGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="2bc1c-103">List macOSGeneralDeviceConfigurations</span></span>

<span data-ttu-id="2bc1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bc1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bc1c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bc1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bc1c-106">Listar propriedades e relações dos objetos [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bc1c-106">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bc1c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bc1c-107">Prerequisites</span></span>
<span data-ttu-id="2bc1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bc1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bc1c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bc1c-110">Permission type</span></span>|<span data-ttu-id="2bc1c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bc1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bc1c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bc1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bc1c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bc1c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2bc1c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bc1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bc1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bc1c-115">Not supported.</span></span>|
|<span data-ttu-id="2bc1c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bc1c-116">Application</span></span>|<span data-ttu-id="2bc1c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bc1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bc1c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bc1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2bc1c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc1c-119">Request headers</span></span>
|<span data-ttu-id="2bc1c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bc1c-120">Header</span></span>|<span data-ttu-id="2bc1c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2bc1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bc1c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bc1c-122">Authorization</span></span>|<span data-ttu-id="2bc1c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bc1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bc1c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bc1c-124">Accept</span></span>|<span data-ttu-id="2bc1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bc1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bc1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc1c-126">Request body</span></span>
<span data-ttu-id="2bc1c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bc1c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc1c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bc1c-128">Response</span></span>
<span data-ttu-id="2bc1c-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bc1c-129">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bc1c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bc1c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bc1c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc1c-131">Request</span></span>
<span data-ttu-id="2bc1c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bc1c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2bc1c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bc1c-133">Response</span></span>
<span data-ttu-id="2bc1c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bc1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




