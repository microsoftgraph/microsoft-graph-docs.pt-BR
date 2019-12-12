---
title: Listar termsAndConditionsAssignments
description: Listar propriedades e relações dos objetos termsAndConditionsAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2737b93698907f9a96c7e0419d1a48149bbcc9cf
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954101"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="76649-103">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="76649-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="76649-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76649-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76649-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76649-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76649-106">Listar propriedades e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="76649-106">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76649-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76649-107">Prerequisites</span></span>
<span data-ttu-id="76649-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76649-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76649-110">Permission type</span></span>|<span data-ttu-id="76649-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76649-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76649-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76649-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76649-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="76649-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="76649-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76649-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76649-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76649-115">Not supported.</span></span>|
|<span data-ttu-id="76649-116">Application</span><span class="sxs-lookup"><span data-stu-id="76649-116">Application</span></span>|<span data-ttu-id="76649-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="76649-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76649-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76649-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="76649-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76649-119">Request headers</span></span>
|<span data-ttu-id="76649-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76649-120">Header</span></span>|<span data-ttu-id="76649-121">Valor</span><span class="sxs-lookup"><span data-stu-id="76649-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76649-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76649-122">Authorization</span></span>|<span data-ttu-id="76649-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76649-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76649-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76649-124">Accept</span></span>|<span data-ttu-id="76649-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76649-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76649-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76649-126">Request body</span></span>
<span data-ttu-id="76649-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76649-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76649-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="76649-128">Response</span></span>
<span data-ttu-id="76649-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76649-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76649-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76649-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="76649-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76649-131">Request</span></span>
<span data-ttu-id="76649-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76649-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="76649-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="76649-133">Response</span></span>
<span data-ttu-id="76649-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76649-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





