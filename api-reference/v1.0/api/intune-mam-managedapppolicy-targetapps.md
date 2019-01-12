---
title: Ação targetApps
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a1efa70963bc35de139422a9af5d57c83a625cfd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915834"
---
# <a name="targetapps-action"></a><span data-ttu-id="fac36-103">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="fac36-103">targetApps action</span></span>

> <span data-ttu-id="fac36-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fac36-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fac36-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fac36-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fac36-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fac36-106">Prerequisites</span></span>
<span data-ttu-id="fac36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fac36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fac36-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fac36-109">Permission type</span></span>|<span data-ttu-id="fac36-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fac36-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fac36-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fac36-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fac36-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fac36-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fac36-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fac36-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fac36-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fac36-114">Not supported.</span></span>|
|<span data-ttu-id="fac36-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fac36-115">Application</span></span>|<span data-ttu-id="fac36-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fac36-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fac36-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fac36-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="fac36-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fac36-118">Request headers</span></span>
|<span data-ttu-id="fac36-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fac36-119">Header</span></span>|<span data-ttu-id="fac36-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fac36-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fac36-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fac36-121">Authorization</span></span>|<span data-ttu-id="fac36-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fac36-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fac36-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fac36-123">Accept</span></span>|<span data-ttu-id="fac36-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fac36-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fac36-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fac36-125">Request body</span></span>
<span data-ttu-id="fac36-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fac36-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fac36-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fac36-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fac36-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fac36-128">Property</span></span>|<span data-ttu-id="fac36-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fac36-129">Type</span></span>|<span data-ttu-id="fac36-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fac36-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fac36-131">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="fac36-131">apps</span></span>|<span data-ttu-id="fac36-132">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fac36-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="fac36-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fac36-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fac36-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fac36-134">Response</span></span>
<span data-ttu-id="fac36-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fac36-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fac36-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fac36-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="fac36-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fac36-137">Request</span></span>
<span data-ttu-id="fac36-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fac36-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

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

### <a name="response"></a><span data-ttu-id="fac36-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fac36-139">Response</span></span>
<span data-ttu-id="fac36-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fac36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



