---
title: Listar termsAndConditionses
description: Listar propriedades e relações dos objetos termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b3ec420ae7f6144d56f6acca1e604599c08a631
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729282"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="76972-103">Listar termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="76972-103">List termsAndConditionses</span></span>

<span data-ttu-id="76972-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76972-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76972-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76972-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76972-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76972-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76972-107">Listar propriedades e relações dos objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="76972-107">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76972-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76972-108">Prerequisites</span></span>
<span data-ttu-id="76972-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76972-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76972-111">Permission type</span></span>|<span data-ttu-id="76972-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76972-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76972-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76972-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76972-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="76972-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="76972-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76972-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76972-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76972-116">Not supported.</span></span>|
|<span data-ttu-id="76972-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76972-117">Application</span></span>|<span data-ttu-id="76972-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="76972-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76972-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76972-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="76972-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76972-120">Request headers</span></span>
|<span data-ttu-id="76972-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76972-121">Header</span></span>|<span data-ttu-id="76972-122">Valor</span><span class="sxs-lookup"><span data-stu-id="76972-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76972-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76972-123">Authorization</span></span>|<span data-ttu-id="76972-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76972-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76972-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76972-125">Accept</span></span>|<span data-ttu-id="76972-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76972-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76972-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76972-127">Request body</span></span>
<span data-ttu-id="76972-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76972-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76972-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="76972-129">Response</span></span>
<span data-ttu-id="76972-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76972-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76972-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76972-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="76972-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76972-132">Request</span></span>
<span data-ttu-id="76972-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76972-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="76972-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="76972-134">Response</span></span>
<span data-ttu-id="76972-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76972-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





