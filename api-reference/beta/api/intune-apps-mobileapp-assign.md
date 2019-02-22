---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b35d89bde14cebdca5333b7e9abaa3a19cba5781
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164187"
---
# <a name="assign-action"></a><span data-ttu-id="9aa40-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="9aa40-103">assign action</span></span>

> <span data-ttu-id="9aa40-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9aa40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9aa40-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9aa40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9aa40-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9aa40-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9aa40-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9aa40-107">Prerequisites</span></span>
<span data-ttu-id="9aa40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9aa40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9aa40-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9aa40-110">Permission type</span></span>|<span data-ttu-id="9aa40-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9aa40-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9aa40-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9aa40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9aa40-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aa40-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9aa40-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9aa40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9aa40-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9aa40-115">Not supported.</span></span>|
|<span data-ttu-id="9aa40-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9aa40-116">Application</span></span>|<span data-ttu-id="9aa40-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9aa40-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9aa40-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9aa40-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="9aa40-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9aa40-119">Request headers</span></span>
|<span data-ttu-id="9aa40-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9aa40-120">Header</span></span>|<span data-ttu-id="9aa40-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9aa40-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9aa40-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9aa40-122">Authorization</span></span>|<span data-ttu-id="9aa40-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9aa40-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9aa40-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9aa40-124">Accept</span></span>|<span data-ttu-id="9aa40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9aa40-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aa40-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9aa40-126">Request body</span></span>
<span data-ttu-id="9aa40-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9aa40-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9aa40-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9aa40-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9aa40-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9aa40-129">Property</span></span>|<span data-ttu-id="9aa40-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aa40-130">Type</span></span>|<span data-ttu-id="9aa40-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aa40-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aa40-132">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="9aa40-132">mobileAppAssignments</span></span>|<span data-ttu-id="9aa40-133">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9aa40-133">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="9aa40-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9aa40-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9aa40-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9aa40-135">Response</span></span>
<span data-ttu-id="9aa40-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9aa40-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9aa40-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9aa40-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="9aa40-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9aa40-138">Request</span></span>
<span data-ttu-id="9aa40-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9aa40-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assign

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

### <a name="response"></a><span data-ttu-id="9aa40-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9aa40-140">Response</span></span>
<span data-ttu-id="9aa40-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9aa40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




