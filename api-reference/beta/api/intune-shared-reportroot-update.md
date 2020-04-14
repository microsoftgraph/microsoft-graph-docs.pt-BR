---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60eba61b9f786cb6a7d5c506558e16eb9e2d5d60
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465387"
---
# <a name="update-reportroot"></a><span data-ttu-id="c26b1-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="c26b1-103">Update reportRoot</span></span>

<span data-ttu-id="c26b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c26b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c26b1-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c26b1-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c26b1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c26b1-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c26b1-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c26b1-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c26b1-108">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="c26b1-108">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c26b1-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c26b1-109">Prerequisites</span></span>
<span data-ttu-id="c26b1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c26b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c26b1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c26b1-112">Permission type</span></span>|<span data-ttu-id="c26b1-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c26b1-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c26b1-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c26b1-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c26b1-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c26b1-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c26b1-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26b1-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c26b1-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="c26b1-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c26b1-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26b1-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c26b1-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c26b1-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c26b1-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c26b1-120">Not supported.</span></span>|
|<span data-ttu-id="c26b1-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c26b1-121">Application</span></span>||
| <span data-ttu-id="c26b1-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c26b1-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c26b1-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26b1-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c26b1-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="c26b1-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c26b1-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26b1-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c26b1-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c26b1-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="c26b1-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c26b1-127">Request headers</span></span>
|<span data-ttu-id="c26b1-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c26b1-128">Header</span></span>|<span data-ttu-id="c26b1-129">Valor</span><span class="sxs-lookup"><span data-stu-id="c26b1-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c26b1-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="c26b1-130">Authorization</span></span>|<span data-ttu-id="c26b1-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c26b1-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c26b1-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c26b1-132">Accept</span></span>|<span data-ttu-id="c26b1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c26b1-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c26b1-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c26b1-134">Request body</span></span>
<span data-ttu-id="c26b1-135">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="c26b1-135">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="c26b1-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="c26b1-136">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="c26b1-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c26b1-137">Property</span></span>|<span data-ttu-id="c26b1-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="c26b1-138">Type</span></span>|<span data-ttu-id="c26b1-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="c26b1-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c26b1-140">id</span><span class="sxs-lookup"><span data-stu-id="c26b1-140">id</span></span>|<span data-ttu-id="c26b1-141">String</span><span class="sxs-lookup"><span data-stu-id="c26b1-141">String</span></span>|<span data-ttu-id="c26b1-142">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="c26b1-142">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c26b1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c26b1-143">Response</span></span>
<span data-ttu-id="c26b1-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c26b1-144">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c26b1-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c26b1-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c26b1-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c26b1-146">Request</span></span>
<span data-ttu-id="c26b1-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c26b1-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="c26b1-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c26b1-148">Response</span></span>
<span data-ttu-id="c26b1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c26b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```









