---
title: Listar policySets
description: Listar propriedades e relações dos objetos policySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6845bca995802293ad3673b9e5c9869c0e618d99
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134589"
---
# <a name="list-policysets"></a><span data-ttu-id="92e0c-103">Listar policySets</span><span class="sxs-lookup"><span data-stu-id="92e0c-103">List policySets</span></span>

<span data-ttu-id="92e0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92e0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92e0c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92e0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e0c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92e0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e0c-107">Listar propriedades e relações dos [objetos policySet.](../resources/intune-policyset-policyset.md)</span><span class="sxs-lookup"><span data-stu-id="92e0c-107">List properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92e0c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92e0c-108">Prerequisites</span></span>
<span data-ttu-id="92e0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92e0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92e0c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92e0c-111">Permission type</span></span>|<span data-ttu-id="92e0c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92e0c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92e0c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92e0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92e0c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e0c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92e0c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92e0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92e0c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92e0c-116">Not supported.</span></span>|
|<span data-ttu-id="92e0c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92e0c-117">Application</span></span>|<span data-ttu-id="92e0c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e0c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92e0c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92e0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets
```

## <a name="request-headers"></a><span data-ttu-id="92e0c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92e0c-120">Request headers</span></span>
|<span data-ttu-id="92e0c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92e0c-121">Header</span></span>|<span data-ttu-id="92e0c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92e0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92e0c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92e0c-123">Authorization</span></span>|<span data-ttu-id="92e0c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92e0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92e0c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92e0c-125">Accept</span></span>|<span data-ttu-id="92e0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92e0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92e0c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92e0c-127">Request body</span></span>
<span data-ttu-id="92e0c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92e0c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92e0c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="92e0c-129">Response</span></span>
<span data-ttu-id="92e0c-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos policySet](../resources/intune-policyset-policyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92e0c-130">If successful, this method returns a `200 OK` response code and a collection of [policySet](../resources/intune-policyset-policyset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92e0c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92e0c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="92e0c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92e0c-132">Request</span></span>
<span data-ttu-id="92e0c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92e0c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets
```

### <a name="response"></a><span data-ttu-id="92e0c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="92e0c-134">Response</span></span>
<span data-ttu-id="92e0c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92e0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 578

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySet",
      "id": "653cb373-b373-653c-73b3-3c6573b33c65",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ],
      "roleScopeTags": [
        "Role Scope Tags value"
      ]
    }
  ]
}
```




