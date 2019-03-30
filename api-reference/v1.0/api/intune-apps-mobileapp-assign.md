---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e82e93f2f5d7c0f95290fdf7c8b0e2ee0abb7abd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988249"
---
# <a name="assign-action"></a><span data-ttu-id="ac730-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="ac730-103">assign action</span></span>

> <span data-ttu-id="ac730-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac730-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac730-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ac730-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac730-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac730-106">Prerequisites</span></span>
<span data-ttu-id="ac730-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac730-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac730-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac730-109">Permission type</span></span>|<span data-ttu-id="ac730-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac730-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac730-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac730-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac730-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac730-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac730-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac730-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac730-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac730-114">Not supported.</span></span>|
|<span data-ttu-id="ac730-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac730-115">Application</span></span>|<span data-ttu-id="ac730-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac730-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac730-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac730-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ac730-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac730-118">Request headers</span></span>
|<span data-ttu-id="ac730-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac730-119">Header</span></span>|<span data-ttu-id="ac730-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ac730-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac730-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac730-121">Authorization</span></span>|<span data-ttu-id="ac730-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac730-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac730-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac730-123">Accept</span></span>|<span data-ttu-id="ac730-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ac730-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac730-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac730-125">Request body</span></span>
<span data-ttu-id="ac730-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ac730-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ac730-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ac730-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ac730-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac730-128">Property</span></span>|<span data-ttu-id="ac730-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac730-129">Type</span></span>|<span data-ttu-id="ac730-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac730-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac730-131">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="ac730-131">mobileAppAssignments</span></span>|<span data-ttu-id="ac730-132">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ac730-132">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="ac730-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ac730-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ac730-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac730-134">Response</span></span>
<span data-ttu-id="ac730-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ac730-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ac730-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac730-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac730-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac730-137">Request</span></span>
<span data-ttu-id="ac730-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac730-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac730-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac730-139">Response</span></span>
<span data-ttu-id="ac730-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac730-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



