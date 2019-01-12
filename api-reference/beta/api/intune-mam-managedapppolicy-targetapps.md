---
title: Ação targetApps
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 248372d64d6e8e42f131fdb78582db00b01f1ee8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944079"
---
# <a name="targetapps-action"></a><span data-ttu-id="8e8f9-103">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="8e8f9-103">targetApps action</span></span>

> <span data-ttu-id="8e8f9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e8f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e8f9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e8f9-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8e8f9-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e8f9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e8f9-108">Prerequisites</span></span>
<span data-ttu-id="8e8f9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e8f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e8f9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e8f9-111">Permission type</span></span>|<span data-ttu-id="8e8f9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e8f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e8f9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e8f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e8f9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e8f9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e8f9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e8f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e8f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-116">Not supported.</span></span>|
|<span data-ttu-id="8e8f9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e8f9-117">Application</span></span>|<span data-ttu-id="8e8f9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e8f9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e8f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="8e8f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8f9-120">Request headers</span></span>
|<span data-ttu-id="8e8f9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e8f9-121">Header</span></span>|<span data-ttu-id="8e8f9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8e8f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e8f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e8f9-123">Authorization</span></span>|<span data-ttu-id="8e8f9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e8f9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e8f9-125">Accept</span></span>|<span data-ttu-id="8e8f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e8f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e8f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8f9-127">Request body</span></span>
<span data-ttu-id="8e8f9-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8e8f9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8e8f9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e8f9-130">Property</span></span>|<span data-ttu-id="8e8f9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e8f9-131">Type</span></span>|<span data-ttu-id="8e8f9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e8f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e8f9-133">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="8e8f9-133">apps</span></span>|<span data-ttu-id="8e8f9-134">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e8f9-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="8e8f9-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8e8f9-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8e8f9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8f9-136">Response</span></span>
<span data-ttu-id="8e8f9-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e8f9-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e8f9-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e8f9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8f9-139">Request</span></span>
<span data-ttu-id="8e8f9-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

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

### <a name="response"></a><span data-ttu-id="8e8f9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8f9-141">Response</span></span>
<span data-ttu-id="8e8f9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e8f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





