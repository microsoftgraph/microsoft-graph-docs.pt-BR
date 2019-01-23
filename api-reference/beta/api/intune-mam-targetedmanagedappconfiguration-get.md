---
title: Acessar targetedManagedAppConfiguration
description: Ler propriedades e relações do objeto targetedManagedAppConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2deff854e237c221aaf8610d43bed761477a6251
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420231"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="f2c55-103">Acessar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2c55-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="f2c55-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2c55-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2c55-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2c55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2c55-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f2c55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2c55-107">Leia as propriedades e as relações do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2c55-107">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2c55-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2c55-108">Prerequisites</span></span>
<span data-ttu-id="f2c55-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2c55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f2c55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2c55-111">Permission type</span></span>|<span data-ttu-id="f2c55-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2c55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2c55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2c55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2c55-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2c55-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f2c55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2c55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2c55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2c55-116">Not supported.</span></span>|
|<span data-ttu-id="f2c55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c55-117">Application</span></span>|<span data-ttu-id="f2c55-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2c55-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2c55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2c55-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2c55-120">Optional query parameters</span></span>
<span data-ttu-id="f2c55-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2c55-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2c55-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c55-122">Request headers</span></span>
|<span data-ttu-id="f2c55-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2c55-123">Header</span></span>|<span data-ttu-id="f2c55-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f2c55-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2c55-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2c55-125">Authorization</span></span>|<span data-ttu-id="f2c55-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2c55-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2c55-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2c55-127">Accept</span></span>|<span data-ttu-id="f2c55-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f2c55-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2c55-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c55-129">Request body</span></span>
<span data-ttu-id="f2c55-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2c55-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2c55-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c55-131">Response</span></span>
<span data-ttu-id="f2c55-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2c55-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2c55-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2c55-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2c55-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c55-134">Request</span></span>
<span data-ttu-id="f2c55-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2c55-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f2c55-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c55-136">Response</span></span>
<span data-ttu-id="f2c55-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2c55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```




