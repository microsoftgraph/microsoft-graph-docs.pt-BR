---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8438faa7367a27d5ee4df605f74426038d1e0f70
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178007"
---
# <a name="assign-action"></a><span data-ttu-id="b6e0d-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b6e0d-103">assign action</span></span>

<span data-ttu-id="b6e0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6e0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6e0d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6e0d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6e0d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6e0d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6e0d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6e0d-108">Prerequisites</span></span>
<span data-ttu-id="b6e0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6e0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6e0d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6e0d-111">Permission type</span></span>|<span data-ttu-id="b6e0d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6e0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6e0d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6e0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6e0d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e0d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6e0d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6e0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6e0d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-116">Not supported.</span></span>|
|<span data-ttu-id="b6e0d-117">Application</span><span class="sxs-lookup"><span data-stu-id="b6e0d-117">Application</span></span>|<span data-ttu-id="b6e0d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e0d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6e0d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6e0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b6e0d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e0d-120">Request headers</span></span>
|<span data-ttu-id="b6e0d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6e0d-121">Header</span></span>|<span data-ttu-id="b6e0d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6e0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6e0d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6e0d-123">Authorization</span></span>|<span data-ttu-id="b6e0d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6e0d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6e0d-125">Accept</span></span>|<span data-ttu-id="b6e0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6e0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6e0d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e0d-127">Request body</span></span>
<span data-ttu-id="b6e0d-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b6e0d-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b6e0d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6e0d-130">Property</span></span>|<span data-ttu-id="b6e0d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6e0d-131">Type</span></span>|<span data-ttu-id="b6e0d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6e0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6e0d-133">assignments</span><span class="sxs-lookup"><span data-stu-id="b6e0d-133">assignments</span></span>|<span data-ttu-id="b6e0d-134">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b6e0d-134">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b6e0d-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6e0d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b6e0d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6e0d-136">Response</span></span>
<span data-ttu-id="b6e0d-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6e0d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6e0d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6e0d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e0d-139">Request</span></span>
<span data-ttu-id="b6e0d-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

Content-type: application/json
Content-length: 287

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b6e0d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6e0d-141">Response</span></span>
<span data-ttu-id="b6e0d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6e0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



