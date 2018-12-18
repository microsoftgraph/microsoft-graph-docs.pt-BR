---
title: Atualizar officeClientConfigurationAssignment
description: Atualize as propriedades de um objeto officeClientConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 78b0ae28bc61bc0d8d8c083502c6f6ef2cf7d0fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343031"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="b0f6a-103">Atualizar officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f6a-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="b0f6a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0f6a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0f6a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0f6a-107">Atualize as propriedades de um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0f6a-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0f6a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0f6a-108">Prerequisites</span></span>
<span data-ttu-id="b0f6a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0f6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0f6a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0f6a-111">Permission type</span></span>|<span data-ttu-id="b0f6a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0f6a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0f6a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0f6a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0f6a-114">\* \* TODO: Determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="b0f6a-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="b0f6a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0f6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0f6a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-116">Not supported.</span></span>|
|<span data-ttu-id="b0f6a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0f6a-117">Application</span></span>|<span data-ttu-id="b0f6a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0f6a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0f6a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b0f6a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0f6a-120">Request headers</span></span>
|<span data-ttu-id="b0f6a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0f6a-121">Header</span></span>|<span data-ttu-id="b0f6a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0f6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0f6a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0f6a-123">Authorization</span></span>|<span data-ttu-id="b0f6a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0f6a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0f6a-125">Accept</span></span>|<span data-ttu-id="b0f6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0f6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0f6a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0f6a-127">Request body</span></span>
<span data-ttu-id="b0f6a-128">No corpo da solicitação, fornece uma representação JSON para o objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0f6a-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b0f6a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b0f6a-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="b0f6a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0f6a-130">Property</span></span>|<span data-ttu-id="b0f6a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0f6a-131">Type</span></span>|<span data-ttu-id="b0f6a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0f6a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0f6a-133">id</span><span class="sxs-lookup"><span data-stu-id="b0f6a-133">id</span></span>|<span data-ttu-id="b0f6a-134">String</span><span class="sxs-lookup"><span data-stu-id="b0f6a-134">String</span></span>|<span data-ttu-id="b0f6a-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b0f6a-135">Not yet documented</span></span>|
|<span data-ttu-id="b0f6a-136">destino</span><span class="sxs-lookup"><span data-stu-id="b0f6a-136">target</span></span>|[<span data-ttu-id="b0f6a-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b0f6a-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="b0f6a-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b0f6a-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b0f6a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0f6a-139">Response</span></span>
<span data-ttu-id="b0f6a-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0f6a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0f6a-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0f6a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0f6a-142">Request</span></span>
<span data-ttu-id="b0f6a-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b0f6a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0f6a-144">Response</span></span>
<span data-ttu-id="b0f6a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0f6a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



