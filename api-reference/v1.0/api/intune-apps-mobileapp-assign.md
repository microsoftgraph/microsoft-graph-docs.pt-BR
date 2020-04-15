---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a5303dac69ec19e8ff47c7be22ac15bddb2538d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447923"
---
# <a name="assign-action"></a><span data-ttu-id="58201-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="58201-103">assign action</span></span>

<span data-ttu-id="58201-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58201-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58201-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58201-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58201-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58201-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58201-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58201-107">Prerequisites</span></span>
<span data-ttu-id="58201-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58201-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58201-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58201-110">Permission type</span></span>|<span data-ttu-id="58201-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58201-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58201-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58201-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58201-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58201-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58201-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58201-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58201-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58201-115">Not supported.</span></span>|
|<span data-ttu-id="58201-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58201-116">Application</span></span>|<span data-ttu-id="58201-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58201-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58201-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58201-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="58201-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58201-119">Request headers</span></span>
|<span data-ttu-id="58201-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58201-120">Header</span></span>|<span data-ttu-id="58201-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58201-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58201-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58201-122">Authorization</span></span>|<span data-ttu-id="58201-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58201-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58201-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58201-124">Accept</span></span>|<span data-ttu-id="58201-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58201-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58201-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58201-126">Request body</span></span>
<span data-ttu-id="58201-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="58201-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="58201-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="58201-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="58201-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58201-129">Property</span></span>|<span data-ttu-id="58201-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="58201-130">Type</span></span>|<span data-ttu-id="58201-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="58201-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58201-132">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="58201-132">mobileAppAssignments</span></span>|<span data-ttu-id="58201-133">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="58201-133">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="58201-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58201-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="58201-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="58201-135">Response</span></span>
<span data-ttu-id="58201-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="58201-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="58201-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58201-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="58201-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58201-138">Request</span></span>
<span data-ttu-id="58201-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58201-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="58201-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="58201-140">Response</span></span>
<span data-ttu-id="58201-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58201-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






