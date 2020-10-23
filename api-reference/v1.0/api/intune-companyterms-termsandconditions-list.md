---
title: Listar termsAndConditions
description: Listar propriedades e relações dos objetos termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db780d4c97e391e4c70c34b5156398421d7fdc71
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733116"
---
# <a name="list-termsandconditions"></a><span data-ttu-id="b2c45-103">Listar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="b2c45-103">List termsAndConditions</span></span>

<span data-ttu-id="b2c45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2c45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2c45-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2c45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2c45-106">Listar propriedades e relações dos objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="b2c45-106">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2c45-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2c45-107">Prerequisites</span></span>
<span data-ttu-id="b2c45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2c45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2c45-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2c45-110">Permission type</span></span>|<span data-ttu-id="b2c45-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2c45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2c45-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2c45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2c45-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2c45-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b2c45-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2c45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2c45-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2c45-115">Not supported.</span></span>|
|<span data-ttu-id="b2c45-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2c45-116">Application</span></span>|<span data-ttu-id="b2c45-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2c45-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2c45-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2c45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="b2c45-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c45-119">Request headers</span></span>
|<span data-ttu-id="b2c45-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2c45-120">Header</span></span>|<span data-ttu-id="b2c45-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2c45-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2c45-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2c45-122">Authorization</span></span>|<span data-ttu-id="b2c45-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2c45-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2c45-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2c45-124">Accept</span></span>|<span data-ttu-id="b2c45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2c45-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2c45-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c45-126">Request body</span></span>
<span data-ttu-id="b2c45-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2c45-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2c45-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c45-128">Response</span></span>
<span data-ttu-id="b2c45-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2c45-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2c45-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2c45-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2c45-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c45-131">Request</span></span>
<span data-ttu-id="b2c45-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2c45-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="b2c45-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c45-133">Response</span></span>
<span data-ttu-id="b2c45-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2c45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









