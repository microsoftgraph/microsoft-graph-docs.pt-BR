---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 019abecc0f9d7560f907652166f8e2ba54cfa2c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974746"
---
# <a name="assign-action"></a><span data-ttu-id="b20ba-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b20ba-103">assign action</span></span>

> <span data-ttu-id="b20ba-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b20ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b20ba-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b20ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b20ba-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b20ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b20ba-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b20ba-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b20ba-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b20ba-108">Prerequisites</span></span>
<span data-ttu-id="b20ba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b20ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b20ba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b20ba-111">Permission type</span></span>|<span data-ttu-id="b20ba-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b20ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b20ba-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b20ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b20ba-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b20ba-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b20ba-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b20ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b20ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b20ba-116">Not supported.</span></span>|
|<span data-ttu-id="b20ba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b20ba-117">Application</span></span>|<span data-ttu-id="b20ba-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b20ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b20ba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b20ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b20ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b20ba-120">Request headers</span></span>
|<span data-ttu-id="b20ba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b20ba-121">Header</span></span>|<span data-ttu-id="b20ba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b20ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b20ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b20ba-123">Authorization</span></span>|<span data-ttu-id="b20ba-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b20ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b20ba-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b20ba-125">Accept</span></span>|<span data-ttu-id="b20ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b20ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b20ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b20ba-127">Request body</span></span>
<span data-ttu-id="b20ba-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b20ba-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b20ba-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b20ba-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b20ba-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b20ba-130">Property</span></span>|<span data-ttu-id="b20ba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b20ba-131">Type</span></span>|<span data-ttu-id="b20ba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b20ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b20ba-133">assignments</span><span class="sxs-lookup"><span data-stu-id="b20ba-133">assignments</span></span>|<span data-ttu-id="b20ba-134">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b20ba-134">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b20ba-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b20ba-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b20ba-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b20ba-136">Response</span></span>
<span data-ttu-id="b20ba-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b20ba-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b20ba-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b20ba-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="b20ba-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b20ba-139">Request</span></span>
<span data-ttu-id="b20ba-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b20ba-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b20ba-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b20ba-141">Response</span></span>
<span data-ttu-id="b20ba-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b20ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





