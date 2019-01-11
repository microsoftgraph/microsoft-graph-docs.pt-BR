---
title: Ação targetApps
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f9e7ceaa79021b1fe3dea5ff9fb0d0080201a3cd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887357"
---
# <a name="targetapps-action"></a><span data-ttu-id="f7f9c-103">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="f7f9c-103">targetApps action</span></span>

> <span data-ttu-id="f7f9c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7f9c-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7f9c-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7f9c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7f9c-106">Prerequisites</span></span>
<span data-ttu-id="f7f9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7f9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7f9c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7f9c-109">Permission type</span></span>|<span data-ttu-id="f7f9c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7f9c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7f9c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7f9c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7f9c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7f9c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7f9c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7f9c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7f9c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-114">Not supported.</span></span>|
|<span data-ttu-id="f7f9c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7f9c-115">Application</span></span>|<span data-ttu-id="f7f9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7f9c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7f9c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="f7f9c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f9c-118">Request headers</span></span>
|<span data-ttu-id="f7f9c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7f9c-119">Header</span></span>|<span data-ttu-id="f7f9c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f7f9c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7f9c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7f9c-121">Authorization</span></span>|<span data-ttu-id="f7f9c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7f9c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7f9c-123">Accept</span></span>|<span data-ttu-id="f7f9c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f7f9c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7f9c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f9c-125">Request body</span></span>
<span data-ttu-id="f7f9c-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f7f9c-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f7f9c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7f9c-128">Property</span></span>|<span data-ttu-id="f7f9c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7f9c-129">Type</span></span>|<span data-ttu-id="f7f9c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7f9c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7f9c-131">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="f7f9c-131">apps</span></span>|<span data-ttu-id="f7f9c-132">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7f9c-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="f7f9c-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7f9c-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7f9c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7f9c-134">Response</span></span>
<span data-ttu-id="f7f9c-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7f9c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7f9c-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7f9c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7f9c-137">Request</span></span>
<span data-ttu-id="f7f9c-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

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

### <a name="response"></a><span data-ttu-id="f7f9c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7f9c-139">Response</span></span>
<span data-ttu-id="f7f9c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7f9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



