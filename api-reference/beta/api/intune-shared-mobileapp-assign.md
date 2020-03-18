---
title: atribuir ação
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f83ec3e1cddbc7a4ba5fc4f513656872f72f4ba5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800806"
---
# <a name="assign-action"></a><span data-ttu-id="60702-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="60702-103">assign action</span></span>

> <span data-ttu-id="60702-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60702-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60702-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60702-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60702-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="60702-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60702-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60702-107">Prerequisites</span></span>
<span data-ttu-id="60702-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60702-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60702-110">Permission type</span></span>|<span data-ttu-id="60702-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60702-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60702-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60702-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="60702-113">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="60702-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="60702-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60702-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60702-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60702-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60702-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60702-116">Not supported.</span></span>|
|<span data-ttu-id="60702-117">Application</span><span class="sxs-lookup"><span data-stu-id="60702-117">Application</span></span>||
| <span data-ttu-id="60702-118">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="60702-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="60702-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60702-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60702-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60702-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="60702-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60702-121">Request headers</span></span>
|<span data-ttu-id="60702-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60702-122">Header</span></span>|<span data-ttu-id="60702-123">Valor</span><span class="sxs-lookup"><span data-stu-id="60702-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60702-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="60702-124">Authorization</span></span>|<span data-ttu-id="60702-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60702-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60702-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60702-126">Accept</span></span>|<span data-ttu-id="60702-127">application/json</span><span class="sxs-lookup"><span data-stu-id="60702-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60702-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60702-128">Request body</span></span>
<span data-ttu-id="60702-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="60702-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="60702-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="60702-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="60702-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60702-131">Property</span></span>|<span data-ttu-id="60702-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="60702-132">Type</span></span>|<span data-ttu-id="60702-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="60702-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60702-134">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="60702-134">mobileAppAssignments</span></span>|<span data-ttu-id="60702-135">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="60702-135">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="60702-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="60702-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="60702-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="60702-137">Response</span></span>
<span data-ttu-id="60702-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="60702-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="60702-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60702-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="60702-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60702-140">Request</span></span>
<span data-ttu-id="60702-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60702-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60702-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="60702-142">Response</span></span>
<span data-ttu-id="60702-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60702-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







