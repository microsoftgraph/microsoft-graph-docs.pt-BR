---
title: Listar iosCertificateProfiles
description: Listar propriedades e relações dos objetos iosCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50ebd03e6c4ac298aae0ef3112a87eb307c1866b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753885"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="90f74-103">Listar iosCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="90f74-103">List iosCertificateProfiles</span></span>

<span data-ttu-id="90f74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90f74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90f74-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90f74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90f74-106">Listar propriedades e relações dos objetos [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="90f74-106">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90f74-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90f74-107">Prerequisites</span></span>
<span data-ttu-id="90f74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90f74-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90f74-110">Permission type</span></span>|<span data-ttu-id="90f74-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90f74-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90f74-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90f74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90f74-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90f74-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90f74-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90f74-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90f74-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90f74-115">Not supported.</span></span>|
|<span data-ttu-id="90f74-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90f74-116">Application</span></span>|<span data-ttu-id="90f74-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90f74-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90f74-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90f74-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90f74-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90f74-119">Request headers</span></span>
|<span data-ttu-id="90f74-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90f74-120">Header</span></span>|<span data-ttu-id="90f74-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90f74-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90f74-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90f74-122">Authorization</span></span>|<span data-ttu-id="90f74-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90f74-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90f74-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90f74-124">Accept</span></span>|<span data-ttu-id="90f74-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90f74-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90f74-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90f74-126">Request body</span></span>
<span data-ttu-id="90f74-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90f74-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90f74-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="90f74-128">Response</span></span>
<span data-ttu-id="90f74-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90f74-129">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90f74-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90f74-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90f74-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90f74-131">Request</span></span>
<span data-ttu-id="90f74-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90f74-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="90f74-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="90f74-133">Response</span></span>
<span data-ttu-id="90f74-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90f74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfile",
      "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




