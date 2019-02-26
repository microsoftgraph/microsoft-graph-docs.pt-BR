---
title: Listar iosCertificateProfiles
description: Listar propriedades e relações dos objetos iosCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf96576d6ef4c349c4f0103c3b2e53d5e0594111
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263564"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="b8712-103">Listar iosCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="b8712-103">List iosCertificateProfiles</span></span>

> <span data-ttu-id="b8712-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8712-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8712-105">Listar propriedades e relações dos objetos [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b8712-105">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8712-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8712-106">Prerequisites</span></span>
<span data-ttu-id="b8712-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b8712-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8712-109">Permission type</span></span>|<span data-ttu-id="b8712-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8712-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8712-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8712-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8712-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8712-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b8712-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8712-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8712-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8712-114">Not supported.</span></span>|
|<span data-ttu-id="b8712-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8712-115">Application</span></span>|<span data-ttu-id="b8712-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8712-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8712-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8712-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8712-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8712-118">Request headers</span></span>
|<span data-ttu-id="b8712-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8712-119">Header</span></span>|<span data-ttu-id="b8712-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b8712-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8712-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8712-121">Authorization</span></span>|<span data-ttu-id="b8712-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8712-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8712-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8712-123">Accept</span></span>|<span data-ttu-id="b8712-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8712-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8712-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8712-125">Request body</span></span>
<span data-ttu-id="b8712-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8712-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8712-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8712-127">Response</span></span>
<span data-ttu-id="b8712-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8712-128">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8712-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8712-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8712-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8712-130">Request</span></span>
<span data-ttu-id="b8712-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8712-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b8712-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8712-132">Response</span></span>
<span data-ttu-id="b8712-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8712-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



