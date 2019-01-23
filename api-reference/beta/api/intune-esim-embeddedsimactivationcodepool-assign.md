---
title: atribuir ação
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: af3952b78c3a3ff00a9b4d43938508f338feea19
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414582"
---
# <a name="assign-action"></a><span data-ttu-id="adef4-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="adef4-103">assign action</span></span>

> <span data-ttu-id="adef4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="adef4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="adef4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="adef4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adef4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="adef4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adef4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="adef4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adef4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="adef4-108">Prerequisites</span></span>
<span data-ttu-id="adef4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="adef4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="adef4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adef4-111">Permission type</span></span>|<span data-ttu-id="adef4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="adef4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adef4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adef4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adef4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adef4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="adef4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adef4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adef4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adef4-116">Not supported.</span></span>|
|<span data-ttu-id="adef4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adef4-117">Application</span></span>|<span data-ttu-id="adef4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adef4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adef4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adef4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="adef4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adef4-120">Request headers</span></span>
|<span data-ttu-id="adef4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="adef4-121">Header</span></span>|<span data-ttu-id="adef4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="adef4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adef4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="adef4-123">Authorization</span></span>|<span data-ttu-id="adef4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adef4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adef4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="adef4-125">Accept</span></span>|<span data-ttu-id="adef4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adef4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adef4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adef4-127">Request body</span></span>
<span data-ttu-id="adef4-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="adef4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="adef4-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="adef4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="adef4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adef4-130">Property</span></span>|<span data-ttu-id="adef4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="adef4-131">Type</span></span>|<span data-ttu-id="adef4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="adef4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adef4-133">assignments</span><span class="sxs-lookup"><span data-stu-id="adef4-133">assignments</span></span>|<span data-ttu-id="adef4-134">coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="adef4-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="adef4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="adef4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="adef4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="adef4-136">Response</span></span>
<span data-ttu-id="adef4-137">Se tiver êxito, essa ação retornará um `200 OK` código de resposta e um conjunto de [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adef4-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adef4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adef4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="adef4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adef4-139">Request</span></span>
<span data-ttu-id="adef4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adef4-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 287

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="adef4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="adef4-141">Response</span></span>
<span data-ttu-id="adef4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adef4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




