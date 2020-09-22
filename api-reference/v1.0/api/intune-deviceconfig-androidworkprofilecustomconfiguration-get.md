---
title: Obter androidWorkProfileCustomConfiguration
description: Leia as propriedades e as relações do objeto androidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b9d87bdc10eee71ca8eb0ae18acc4cc005dc9a3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985388"
---
# <a name="get-androidworkprofilecustomconfiguration"></a><span data-ttu-id="2658b-103">Obter androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="2658b-103">Get androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="2658b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2658b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2658b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2658b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2658b-106">Leia as propriedades e as relações do objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2658b-106">Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2658b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2658b-107">Prerequisites</span></span>
<span data-ttu-id="2658b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2658b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2658b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2658b-110">Permission type</span></span>|<span data-ttu-id="2658b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2658b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2658b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2658b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2658b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2658b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2658b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2658b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2658b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2658b-115">Not supported.</span></span>|
|<span data-ttu-id="2658b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2658b-116">Application</span></span>|<span data-ttu-id="2658b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2658b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2658b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2658b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2658b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2658b-119">Optional query parameters</span></span>
<span data-ttu-id="2658b-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2658b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2658b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2658b-121">Request headers</span></span>
|<span data-ttu-id="2658b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2658b-122">Header</span></span>|<span data-ttu-id="2658b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2658b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2658b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2658b-124">Authorization</span></span>|<span data-ttu-id="2658b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2658b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2658b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2658b-126">Accept</span></span>|<span data-ttu-id="2658b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2658b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2658b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2658b-128">Request body</span></span>
<span data-ttu-id="2658b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2658b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2658b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2658b-130">Response</span></span>
<span data-ttu-id="2658b-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2658b-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2658b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2658b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2658b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2658b-133">Request</span></span>
<span data-ttu-id="2658b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2658b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2658b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2658b-135">Response</span></span>
<span data-ttu-id="2658b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2658b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
    "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```









