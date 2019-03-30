---
title: Acessar iosCertificateProfile
description: Leia as propriedades e as relações do objeto iosCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f4cf567d8dbc9d7961536b676a1e8388a355337
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985715"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="0b05c-103">Acessar iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0b05c-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="0b05c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b05c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b05c-105">Leia as propriedades e as relações do objeto [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0b05c-105">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b05c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b05c-106">Prerequisites</span></span>
<span data-ttu-id="0b05c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b05c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b05c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b05c-109">Permission type</span></span>|<span data-ttu-id="0b05c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b05c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b05c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b05c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b05c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b05c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0b05c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b05c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b05c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b05c-114">Not supported.</span></span>|
|<span data-ttu-id="0b05c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b05c-115">Application</span></span>|<span data-ttu-id="0b05c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b05c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b05c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b05c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b05c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b05c-118">Optional query parameters</span></span>
<span data-ttu-id="0b05c-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0b05c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b05c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b05c-120">Request headers</span></span>
|<span data-ttu-id="0b05c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b05c-121">Header</span></span>|<span data-ttu-id="0b05c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0b05c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b05c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b05c-123">Authorization</span></span>|<span data-ttu-id="0b05c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b05c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b05c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b05c-125">Accept</span></span>|<span data-ttu-id="0b05c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b05c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b05c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b05c-127">Request body</span></span>
<span data-ttu-id="0b05c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b05c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b05c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b05c-129">Response</span></span>
<span data-ttu-id="0b05c-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b05c-130">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b05c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b05c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b05c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b05c-132">Request</span></span>
<span data-ttu-id="0b05c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b05c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0b05c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b05c-134">Response</span></span>
<span data-ttu-id="0b05c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b05c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



