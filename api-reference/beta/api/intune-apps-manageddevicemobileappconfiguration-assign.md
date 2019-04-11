---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff737c30b5ceab47882375110a2601d021d5652b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794642"
---
# <a name="assign-action"></a><span data-ttu-id="43084-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="43084-103">assign action</span></span>

> <span data-ttu-id="43084-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43084-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43084-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43084-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43084-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="43084-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43084-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43084-107">Prerequisites</span></span>
<span data-ttu-id="43084-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43084-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43084-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43084-110">Permission type</span></span>|<span data-ttu-id="43084-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43084-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43084-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43084-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43084-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43084-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43084-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43084-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43084-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43084-115">Not supported.</span></span>|
|<span data-ttu-id="43084-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43084-116">Application</span></span>|<span data-ttu-id="43084-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43084-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43084-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43084-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="43084-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43084-119">Request headers</span></span>
|<span data-ttu-id="43084-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43084-120">Header</span></span>|<span data-ttu-id="43084-121">Valor</span><span class="sxs-lookup"><span data-stu-id="43084-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43084-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43084-122">Authorization</span></span>|<span data-ttu-id="43084-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43084-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43084-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43084-124">Accept</span></span>|<span data-ttu-id="43084-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43084-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43084-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43084-126">Request body</span></span>
<span data-ttu-id="43084-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="43084-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="43084-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="43084-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="43084-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43084-129">Property</span></span>|<span data-ttu-id="43084-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="43084-130">Type</span></span>|<span data-ttu-id="43084-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="43084-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43084-132">assignments</span><span class="sxs-lookup"><span data-stu-id="43084-132">assignments</span></span>|<span data-ttu-id="43084-133">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="43084-133">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="43084-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="43084-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43084-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="43084-135">Response</span></span>
<span data-ttu-id="43084-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="43084-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43084-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43084-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="43084-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43084-138">Request</span></span>
<span data-ttu-id="43084-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43084-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

Content-type: application/json
Content-length: 293

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="43084-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="43084-140">Response</span></span>
<span data-ttu-id="43084-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43084-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





