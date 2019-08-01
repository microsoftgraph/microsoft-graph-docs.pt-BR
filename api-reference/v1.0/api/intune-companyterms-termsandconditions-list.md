---
title: Listar termsAndConditionses
description: Listar propriedades e relações dos objetos termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e10c75da24a534459e44d50a17c99a3453dd197
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019819"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="a1749-103">Listar termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="a1749-103">List termsAndConditionses</span></span>

> <span data-ttu-id="a1749-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1749-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1749-105">Listar propriedades e relações dos objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a1749-105">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1749-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1749-106">Prerequisites</span></span>
<span data-ttu-id="a1749-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1749-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1749-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1749-109">Permission type</span></span>|<span data-ttu-id="a1749-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1749-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1749-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1749-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1749-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1749-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a1749-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1749-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1749-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1749-114">Not supported.</span></span>|
|<span data-ttu-id="a1749-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1749-115">Application</span></span>|<span data-ttu-id="a1749-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1749-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1749-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1749-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="a1749-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1749-118">Request headers</span></span>
|<span data-ttu-id="a1749-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1749-119">Header</span></span>|<span data-ttu-id="a1749-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a1749-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1749-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1749-121">Authorization</span></span>|<span data-ttu-id="a1749-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1749-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1749-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1749-123">Accept</span></span>|<span data-ttu-id="a1749-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1749-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1749-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1749-125">Request body</span></span>
<span data-ttu-id="a1749-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1749-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1749-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1749-127">Response</span></span>
<span data-ttu-id="a1749-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1749-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1749-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1749-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1749-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1749-130">Request</span></span>
<span data-ttu-id="a1749-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1749-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="a1749-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1749-132">Response</span></span>
<span data-ttu-id="a1749-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1749-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```



