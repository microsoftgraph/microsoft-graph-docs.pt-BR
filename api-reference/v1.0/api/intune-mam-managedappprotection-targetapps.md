---
title: Ação targetApps
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: ef8623efc272d4812bb1430bebd41f02effdb2a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303483"
---
# <a name="targetapps-action"></a><span data-ttu-id="d81c7-103">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="d81c7-103">targetApps action</span></span>

> <span data-ttu-id="d81c7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d81c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d81c7-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d81c7-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d81c7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d81c7-106">Prerequisites</span></span>
<span data-ttu-id="d81c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d81c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d81c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d81c7-109">Permission type</span></span>|<span data-ttu-id="d81c7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d81c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d81c7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d81c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d81c7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81c7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d81c7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d81c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d81c7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d81c7-114">Not supported.</span></span>|
|<span data-ttu-id="d81c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d81c7-115">Application</span></span>|<span data-ttu-id="d81c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d81c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d81c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d81c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="d81c7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d81c7-118">Request headers</span></span>
|<span data-ttu-id="d81c7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d81c7-119">Header</span></span>|<span data-ttu-id="d81c7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d81c7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d81c7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d81c7-121">Authorization</span></span>|<span data-ttu-id="d81c7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d81c7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d81c7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d81c7-123">Accept</span></span>|<span data-ttu-id="d81c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d81c7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d81c7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d81c7-125">Request body</span></span>
<span data-ttu-id="d81c7-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d81c7-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d81c7-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d81c7-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d81c7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d81c7-128">Property</span></span>|<span data-ttu-id="d81c7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d81c7-129">Type</span></span>|<span data-ttu-id="d81c7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d81c7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d81c7-131">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="d81c7-131">apps</span></span>|<span data-ttu-id="d81c7-132">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d81c7-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="d81c7-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d81c7-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d81c7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81c7-134">Response</span></span>
<span data-ttu-id="d81c7-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d81c7-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d81c7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d81c7-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="d81c7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d81c7-137">Request</span></span>
<span data-ttu-id="d81c7-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d81c7-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d81c7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81c7-139">Response</span></span>
<span data-ttu-id="d81c7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d81c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



