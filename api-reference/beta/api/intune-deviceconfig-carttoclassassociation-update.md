---
title: Atualizar cartToClassAssociation
description: Atualize as propriedades de um objeto cartToClassAssociation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a140aa3e14895cf0fc7dd5ca2be54afdb1d86052
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967676"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="8d1b9-103">Atualizar cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="8d1b9-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="8d1b9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d1b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d1b9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d1b9-107">Atualize as propriedades de um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="8d1b9-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d1b9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d1b9-108">Prerequisites</span></span>
<span data-ttu-id="8d1b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d1b9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d1b9-111">Permission type</span></span>|<span data-ttu-id="8d1b9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d1b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d1b9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d1b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d1b9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d1b9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d1b9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d1b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d1b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-116">Not supported.</span></span>|
|<span data-ttu-id="8d1b9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d1b9-117">Application</span></span>|<span data-ttu-id="8d1b9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d1b9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="8d1b9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b9-120">Request headers</span></span>
|<span data-ttu-id="8d1b9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d1b9-121">Header</span></span>|<span data-ttu-id="8d1b9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8d1b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d1b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d1b9-123">Authorization</span></span>|<span data-ttu-id="8d1b9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d1b9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d1b9-125">Accept</span></span>|<span data-ttu-id="8d1b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d1b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d1b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b9-127">Request body</span></span>
<span data-ttu-id="8d1b9-128">No corpo da solicitação, fornece uma representação JSON para o objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="8d1b9-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="8d1b9-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span><span class="sxs-lookup"><span data-stu-id="8d1b9-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="8d1b9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d1b9-130">Property</span></span>|<span data-ttu-id="8d1b9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d1b9-131">Type</span></span>|<span data-ttu-id="8d1b9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d1b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d1b9-133">id</span><span class="sxs-lookup"><span data-stu-id="8d1b9-133">id</span></span>|<span data-ttu-id="8d1b9-134">String</span><span class="sxs-lookup"><span data-stu-id="8d1b9-134">String</span></span>|<span data-ttu-id="8d1b9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-135">Key of the entity.</span></span>|
|<span data-ttu-id="8d1b9-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d1b9-136">createdDateTime</span></span>|<span data-ttu-id="8d1b9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d1b9-137">DateTimeOffset</span></span>|<span data-ttu-id="8d1b9-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="8d1b9-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d1b9-139">lastModifiedDateTime</span></span>|<span data-ttu-id="8d1b9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d1b9-140">DateTimeOffset</span></span>|<span data-ttu-id="8d1b9-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8d1b9-142">version</span><span class="sxs-lookup"><span data-stu-id="8d1b9-142">version</span></span>|<span data-ttu-id="8d1b9-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8d1b9-143">Int32</span></span>|<span data-ttu-id="8d1b9-144">Versão do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="8d1b9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8d1b9-145">displayName</span></span>|<span data-ttu-id="8d1b9-146">String</span><span class="sxs-lookup"><span data-stu-id="8d1b9-146">String</span></span>|<span data-ttu-id="8d1b9-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8d1b9-148">description</span><span class="sxs-lookup"><span data-stu-id="8d1b9-148">description</span></span>|<span data-ttu-id="8d1b9-149">String</span><span class="sxs-lookup"><span data-stu-id="8d1b9-149">String</span></span>|<span data-ttu-id="8d1b9-150">Admin fornecido descrição do que o CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="8d1b9-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="8d1b9-151">deviceCartIds</span></span>|<span data-ttu-id="8d1b9-152">String collection</span><span class="sxs-lookup"><span data-stu-id="8d1b9-152">String collection</span></span>|<span data-ttu-id="8d1b9-153">Identificadores de carrinhos de dispositivo a ser associado a classes.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="8d1b9-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="8d1b9-154">classroomIds</span></span>|<span data-ttu-id="8d1b9-155">String collection</span><span class="sxs-lookup"><span data-stu-id="8d1b9-155">String collection</span></span>|<span data-ttu-id="8d1b9-156">Identificadores de salas a ser associado ao dispositivo carrinhos de.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="8d1b9-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d1b9-157">Response</span></span>
<span data-ttu-id="8d1b9-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d1b9-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d1b9-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d1b9-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b9-160">Request</span></span>
<span data-ttu-id="8d1b9-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
Content-type: application/json
Content-length: 274

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8d1b9-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d1b9-162">Response</span></span>
<span data-ttu-id="8d1b9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```





