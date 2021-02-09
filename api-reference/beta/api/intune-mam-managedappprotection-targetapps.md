---
title: Ação targetApps
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cf2db211b37993cb68ae40f5024f0c77110b96a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157915"
---
# <a name="targetapps-action"></a><span data-ttu-id="b0b2f-103">ação targetApps</span><span class="sxs-lookup"><span data-stu-id="b0b2f-103">targetApps action</span></span>

<span data-ttu-id="b0b2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0b2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0b2f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0b2f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0b2f-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b0b2f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0b2f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0b2f-108">Prerequisites</span></span>
<span data-ttu-id="b0b2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0b2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0b2f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0b2f-111">Permission type</span></span>|<span data-ttu-id="b0b2f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0b2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0b2f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0b2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0b2f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0b2f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b0b2f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0b2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0b2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-116">Not supported.</span></span>|
|<span data-ttu-id="b0b2f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0b2f-117">Application</span></span>|<span data-ttu-id="b0b2f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0b2f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0b2f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0b2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="b0b2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0b2f-120">Request headers</span></span>
|<span data-ttu-id="b0b2f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0b2f-121">Header</span></span>|<span data-ttu-id="b0b2f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0b2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0b2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0b2f-123">Authorization</span></span>|<span data-ttu-id="b0b2f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0b2f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0b2f-125">Accept</span></span>|<span data-ttu-id="b0b2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0b2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0b2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0b2f-127">Request body</span></span>
<span data-ttu-id="b0b2f-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b0b2f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b0b2f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0b2f-130">Property</span></span>|<span data-ttu-id="b0b2f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0b2f-131">Type</span></span>|<span data-ttu-id="b0b2f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0b2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0b2f-133">apps</span><span class="sxs-lookup"><span data-stu-id="b0b2f-133">apps</span></span>|<span data-ttu-id="b0b2f-134">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b2f-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="b0b2f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b0b2f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b0b2f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0b2f-136">Response</span></span>
<span data-ttu-id="b0b2f-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b0b2f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0b2f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0b2f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0b2f-139">Request</span></span>
<span data-ttu-id="b0b2f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 336

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b0b2f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0b2f-141">Response</span></span>
<span data-ttu-id="b0b2f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0b2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




