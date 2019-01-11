---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cdfc5fc08151cc4115e6abd95265c7fbc7256c96
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878502"
---
# <a name="assign-action"></a><span data-ttu-id="71944-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="71944-103">assign action</span></span>

> <span data-ttu-id="71944-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="71944-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71944-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="71944-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71944-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="71944-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71944-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="71944-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71944-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71944-108">Prerequisites</span></span>
<span data-ttu-id="71944-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71944-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71944-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71944-111">Permission type</span></span>|<span data-ttu-id="71944-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71944-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71944-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71944-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71944-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71944-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71944-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71944-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71944-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71944-116">Not supported.</span></span>|
|<span data-ttu-id="71944-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71944-117">Application</span></span>|<span data-ttu-id="71944-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71944-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71944-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71944-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="71944-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71944-120">Request headers</span></span>
|<span data-ttu-id="71944-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71944-121">Header</span></span>|<span data-ttu-id="71944-122">Valor</span><span class="sxs-lookup"><span data-stu-id="71944-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71944-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71944-123">Authorization</span></span>|<span data-ttu-id="71944-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71944-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71944-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71944-125">Accept</span></span>|<span data-ttu-id="71944-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71944-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71944-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71944-127">Request body</span></span>
<span data-ttu-id="71944-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="71944-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="71944-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="71944-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="71944-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71944-130">Property</span></span>|<span data-ttu-id="71944-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="71944-131">Type</span></span>|<span data-ttu-id="71944-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71944-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71944-133">assignments</span><span class="sxs-lookup"><span data-stu-id="71944-133">assignments</span></span>|<span data-ttu-id="71944-134">Coleção [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="71944-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="71944-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="71944-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="71944-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="71944-136">Response</span></span>
<span data-ttu-id="71944-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="71944-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="71944-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71944-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="71944-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71944-139">Request</span></span>
<span data-ttu-id="71944-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71944-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="71944-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="71944-141">Response</span></span>
<span data-ttu-id="71944-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71944-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





