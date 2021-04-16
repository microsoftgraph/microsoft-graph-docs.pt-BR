---
title: Ação targetApps
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5dba5d7e6127ae59b01c35e9a80cce13e51a66cd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865387"
---
# <a name="targetapps-action"></a><span data-ttu-id="ec1bb-103">ação targetApps</span><span class="sxs-lookup"><span data-stu-id="ec1bb-103">targetApps action</span></span>

<span data-ttu-id="ec1bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec1bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec1bb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec1bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec1bb-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ec1bb-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec1bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec1bb-108">Prerequisites</span></span>
<span data-ttu-id="ec1bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec1bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec1bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec1bb-111">Permission type</span></span>|<span data-ttu-id="ec1bb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec1bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec1bb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec1bb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ec1bb-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="ec1bb-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ec1bb-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec1bb-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec1bb-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec1bb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec1bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-117">Not supported.</span></span>|
|<span data-ttu-id="ec1bb-118">Application</span><span class="sxs-lookup"><span data-stu-id="ec1bb-118">Application</span></span>||
| <span data-ttu-id="ec1bb-119">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="ec1bb-119">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ec1bb-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec1bb-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec1bb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec1bb-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="ec1bb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec1bb-122">Request headers</span></span>
|<span data-ttu-id="ec1bb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec1bb-123">Header</span></span>|<span data-ttu-id="ec1bb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ec1bb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec1bb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec1bb-125">Authorization</span></span>|<span data-ttu-id="ec1bb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec1bb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec1bb-127">Accept</span></span>|<span data-ttu-id="ec1bb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ec1bb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec1bb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec1bb-129">Request body</span></span>
<span data-ttu-id="ec1bb-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ec1bb-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ec1bb-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec1bb-132">Property</span></span>|<span data-ttu-id="ec1bb-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec1bb-133">Type</span></span>|<span data-ttu-id="ec1bb-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec1bb-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec1bb-135">apps</span><span class="sxs-lookup"><span data-stu-id="ec1bb-135">apps</span></span>|<span data-ttu-id="ec1bb-136">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec1bb-136">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="ec1bb-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ec1bb-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ec1bb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec1bb-138">Response</span></span>
<span data-ttu-id="ec1bb-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ec1bb-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec1bb-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec1bb-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec1bb-141">Request</span></span>
<span data-ttu-id="ec1bb-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec1bb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec1bb-143">Response</span></span>
<span data-ttu-id="ec1bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec1bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







