---
title: Get macOSGeneralDeviceConfiguration
description: Ler propriedades e relações do objeto macOSGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: 6ed46c223529d0dde59750db0ed135b71c08482f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359112"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="bfaac-103">Get macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfaac-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="bfaac-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bfaac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfaac-105">Ler propriedades e relações do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfaac-105">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bfaac-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bfaac-106">Prerequisites</span></span>
<span data-ttu-id="bfaac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfaac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfaac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfaac-109">Permission type</span></span>|<span data-ttu-id="bfaac-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bfaac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfaac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfaac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bfaac-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfaac-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bfaac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfaac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfaac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfaac-114">Not supported.</span></span>|
|<span data-ttu-id="bfaac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfaac-115">Application</span></span>|<span data-ttu-id="bfaac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfaac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfaac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfaac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bfaac-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bfaac-118">Optional query parameters</span></span>
<span data-ttu-id="bfaac-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bfaac-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bfaac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfaac-120">Request headers</span></span>
|<span data-ttu-id="bfaac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bfaac-121">Header</span></span>|<span data-ttu-id="bfaac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bfaac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfaac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfaac-123">Authorization</span></span>|<span data-ttu-id="bfaac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfaac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfaac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bfaac-125">Accept</span></span>|<span data-ttu-id="bfaac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bfaac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfaac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfaac-127">Request body</span></span>
<span data-ttu-id="bfaac-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bfaac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfaac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfaac-129">Response</span></span>
<span data-ttu-id="bfaac-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfaac-130">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfaac-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfaac-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bfaac-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfaac-132">Request</span></span>
<span data-ttu-id="bfaac-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfaac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bfaac-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfaac-134">Response</span></span>
<span data-ttu-id="bfaac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfaac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1155

{
  "value": {
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
}
```



