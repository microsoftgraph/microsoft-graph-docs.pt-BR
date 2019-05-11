---
title: Listar iosCertificateProfiles
description: Listar propriedades e relações dos objetos iosCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ed58fe7ffe0eacf44d696754cbf6b39a409e617
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33926744"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="78e39-103">Listar iosCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="78e39-103">List iosCertificateProfiles</span></span>

> <span data-ttu-id="78e39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78e39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78e39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e39-106">Listar propriedades e relações dos objetos [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="78e39-106">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78e39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78e39-107">Prerequisites</span></span>
<span data-ttu-id="78e39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78e39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78e39-110">Permission type</span></span>|<span data-ttu-id="78e39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78e39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78e39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78e39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78e39-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78e39-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="78e39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78e39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78e39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78e39-115">Not supported.</span></span>|
|<span data-ttu-id="78e39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78e39-116">Application</span></span>|<span data-ttu-id="78e39-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78e39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78e39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78e39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="78e39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78e39-119">Request headers</span></span>
|<span data-ttu-id="78e39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78e39-120">Header</span></span>|<span data-ttu-id="78e39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="78e39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78e39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="78e39-122">Authorization</span></span>|<span data-ttu-id="78e39-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78e39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78e39-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78e39-124">Accept</span></span>|<span data-ttu-id="78e39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78e39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78e39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78e39-126">Request body</span></span>
<span data-ttu-id="78e39-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78e39-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78e39-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e39-128">Response</span></span>
<span data-ttu-id="78e39-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78e39-129">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e39-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78e39-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="78e39-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78e39-131">Request</span></span>
<span data-ttu-id="78e39-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78e39-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="78e39-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e39-133">Response</span></span>
<span data-ttu-id="78e39-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78e39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfile",
      "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




