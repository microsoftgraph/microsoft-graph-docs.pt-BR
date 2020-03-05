---
title: Listar termsAndConditionses
description: Listar propriedades e relações dos objetos termsAndConditions.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf1c7bd1a744677cf121c9fc82145d3cc8123889
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444361"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="7c376-103">Listar termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="7c376-103">List termsAndConditionses</span></span>

<span data-ttu-id="7c376-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7c376-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c376-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c376-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c376-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c376-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c376-107">Listar propriedades e relações dos objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="7c376-107">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c376-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c376-108">Prerequisites</span></span>
<span data-ttu-id="7c376-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c376-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c376-111">Permission type</span></span>|<span data-ttu-id="7c376-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c376-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c376-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c376-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c376-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c376-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7c376-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c376-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c376-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c376-116">Not supported.</span></span>|
|<span data-ttu-id="7c376-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c376-117">Application</span></span>|<span data-ttu-id="7c376-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c376-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c376-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c376-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="7c376-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c376-120">Request headers</span></span>
|<span data-ttu-id="7c376-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c376-121">Header</span></span>|<span data-ttu-id="7c376-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7c376-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c376-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c376-123">Authorization</span></span>|<span data-ttu-id="7c376-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c376-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c376-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c376-125">Accept</span></span>|<span data-ttu-id="7c376-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c376-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c376-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c376-127">Request body</span></span>
<span data-ttu-id="7c376-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c376-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c376-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c376-129">Response</span></span>
<span data-ttu-id="7c376-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c376-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c376-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c376-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c376-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c376-132">Request</span></span>
<span data-ttu-id="7c376-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c376-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="7c376-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c376-134">Response</span></span>
<span data-ttu-id="7c376-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c376-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 656

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```





