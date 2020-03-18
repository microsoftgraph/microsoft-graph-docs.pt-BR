---
title: Ação targetApps
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04e13d90392f5f83abfc4c17137f1e173a026f86
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800610"
---
# <a name="targetapps-action"></a><span data-ttu-id="42806-103">ação targetApps</span><span class="sxs-lookup"><span data-stu-id="42806-103">targetApps action</span></span>

> <span data-ttu-id="42806-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42806-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42806-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42806-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42806-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="42806-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42806-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42806-107">Prerequisites</span></span>
<span data-ttu-id="42806-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42806-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42806-110">Permission type</span></span>|<span data-ttu-id="42806-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42806-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42806-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42806-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="42806-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="42806-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="42806-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42806-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42806-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42806-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42806-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42806-116">Not supported.</span></span>|
|<span data-ttu-id="42806-117">Application</span><span class="sxs-lookup"><span data-stu-id="42806-117">Application</span></span>||
| <span data-ttu-id="42806-118">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="42806-118">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="42806-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42806-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42806-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42806-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="42806-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42806-121">Request headers</span></span>
|<span data-ttu-id="42806-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42806-122">Header</span></span>|<span data-ttu-id="42806-123">Valor</span><span class="sxs-lookup"><span data-stu-id="42806-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42806-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="42806-124">Authorization</span></span>|<span data-ttu-id="42806-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42806-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42806-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42806-126">Accept</span></span>|<span data-ttu-id="42806-127">application/json</span><span class="sxs-lookup"><span data-stu-id="42806-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42806-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42806-128">Request body</span></span>
<span data-ttu-id="42806-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="42806-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="42806-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="42806-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="42806-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42806-131">Property</span></span>|<span data-ttu-id="42806-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="42806-132">Type</span></span>|<span data-ttu-id="42806-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="42806-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42806-134">apps</span><span class="sxs-lookup"><span data-stu-id="42806-134">apps</span></span>|<span data-ttu-id="42806-135">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42806-135">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="42806-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="42806-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42806-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="42806-137">Response</span></span>
<span data-ttu-id="42806-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="42806-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42806-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42806-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="42806-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42806-140">Request</span></span>
<span data-ttu-id="42806-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42806-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="42806-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="42806-142">Response</span></span>
<span data-ttu-id="42806-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42806-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







