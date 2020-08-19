---
title: Enviar comando do dispositivo
description: 'Essa API permite que os recursos do Project Roma para o comando um dispositivo associado a uma conta da Microsoft. Depois de obter uma chamada GET `me/devices` , passe a ID do dispositivo para emitir um comando para seu dispositivo. Há suporte para dois tipos de comandos: LaunchURI e AppServices. Se você estiver usando o LaunchURI, especifique os parâmetros *Type* e *Payload* . Para uma chamada serviço, especifique o '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ailae
ms.openlocfilehash: 73f725dde241e5fc37ace2bc6b5ac92e5401a9fc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812559"
---
# <a name="send-device-command"></a><span data-ttu-id="c9f71-107">Enviar comando do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9f71-107">Send device command</span></span>

<span data-ttu-id="c9f71-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9f71-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9f71-109">Essa API permite que os recursos do Project Roma para o comando um dispositivo associado a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c9f71-109">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="c9f71-110">Depois de obter uma chamada GET `me/devices` , passe a ID do dispositivo para emitir um comando para seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c9f71-110">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="c9f71-111">Há suporte para dois tipos de comandos: LaunchURI e AppServices.</span><span class="sxs-lookup"><span data-stu-id="c9f71-111">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="c9f71-112">Se você estiver usando o LaunchURI, especifique os parâmetros *Type* e *Payload* .</span><span class="sxs-lookup"><span data-stu-id="c9f71-112">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="c9f71-113">Para uma chamada serviço, especifique os parâmetros *Type*, *Payload*, *packageFamilyName*e *appServiceName* .</span><span class="sxs-lookup"><span data-stu-id="c9f71-113">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9f71-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9f71-114">Permissions</span></span>

<span data-ttu-id="c9f71-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9f71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c9f71-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9f71-117">Permission type</span></span>      | <span data-ttu-id="c9f71-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9f71-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9f71-119">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9f71-119">Delegated (work or school account)</span></span> | <span data-ttu-id="c9f71-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9f71-120">Not supported.</span></span>    |
|<span data-ttu-id="c9f71-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9f71-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9f71-122">Device.Command</span><span class="sxs-lookup"><span data-stu-id="c9f71-122">Device.Command</span></span>    |
|<span data-ttu-id="c9f71-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9f71-123">Application</span></span> | <span data-ttu-id="c9f71-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9f71-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9f71-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9f71-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="c9f71-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f71-126">Request headers</span></span>


| <span data-ttu-id="c9f71-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9f71-127">Header</span></span> |<span data-ttu-id="c9f71-128">Valor</span><span class="sxs-lookup"><span data-stu-id="c9f71-128">Value</span></span>
|:----|:------|
|<span data-ttu-id="c9f71-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9f71-129">Authorization</span></span>| <span data-ttu-id="c9f71-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9f71-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c9f71-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9f71-132">Accept</span></span> | <span data-ttu-id="c9f71-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c9f71-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9f71-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f71-134">Request body</span></span>

<span data-ttu-id="c9f71-135">No corpo da solicitação, forneça uma representação JSON das propriedades do comando.</span><span class="sxs-lookup"><span data-stu-id="c9f71-135">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="c9f71-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9f71-136">Response</span></span>

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
### <a name="command-properties"></a><span data-ttu-id="c9f71-137">Propriedades de comando</span><span class="sxs-lookup"><span data-stu-id="c9f71-137">Command properties</span></span>

|<span data-ttu-id="c9f71-138">**Nome**</span><span class="sxs-lookup"><span data-stu-id="c9f71-138">**Name**</span></span>|<span data-ttu-id="c9f71-139">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="c9f71-139">**Type**</span></span>|<span data-ttu-id="c9f71-140">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9f71-140">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="c9f71-141">payload</span><span class="sxs-lookup"><span data-stu-id="c9f71-141">payload</span></span> | <span data-ttu-id="c9f71-142">microsoft.graph.jsem</span><span class="sxs-lookup"><span data-stu-id="c9f71-142">microsoft.graph.json</span></span>| <span data-ttu-id="c9f71-143">Carga a ser enviada a um serviço de aplicativo ou para iniciar um URI em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c9f71-143">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="c9f71-144">responsePayload</span><span class="sxs-lookup"><span data-stu-id="c9f71-144">responsePayload</span></span> | <span data-ttu-id="c9f71-145">microsoft.graph.jsem</span><span class="sxs-lookup"><span data-stu-id="c9f71-145">microsoft.graph.json</span></span>| <span data-ttu-id="c9f71-146">Carga retornada do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="c9f71-146">Payload returned from target device.</span></span> |
|<span data-ttu-id="c9f71-147">postBackURI</span><span class="sxs-lookup"><span data-stu-id="c9f71-147">postBackURI</span></span> | <span data-ttu-id="c9f71-148">String</span><span class="sxs-lookup"><span data-stu-id="c9f71-148">String</span></span> | <span data-ttu-id="c9f71-149">Postar URI para enviar notificações de atualizações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="c9f71-149">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="c9f71-150">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="c9f71-150">packageFamilyName</span></span> | <span data-ttu-id="c9f71-151">String</span><span class="sxs-lookup"><span data-stu-id="c9f71-151">String</span></span> | <span data-ttu-id="c9f71-152">Nome do aplicativo da família de pacote do Windows.</span><span class="sxs-lookup"><span data-stu-id="c9f71-152">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="c9f71-153">appServiceName</span><span class="sxs-lookup"><span data-stu-id="c9f71-153">appServiceName</span></span> | <span data-ttu-id="c9f71-154">String</span><span class="sxs-lookup"><span data-stu-id="c9f71-154">String</span></span> | <span data-ttu-id="c9f71-155">Nome do serviço de aplicativo definido pelo aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="c9f71-155">Name of app service defined by the target application.</span></span> <span data-ttu-id="c9f71-156">Necessário se iniciar um serviço de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9f71-156">Required if launching an app service.</span></span> |
|<span data-ttu-id="c9f71-157">type</span><span class="sxs-lookup"><span data-stu-id="c9f71-157">type</span></span>| <span data-ttu-id="c9f71-158">String</span><span class="sxs-lookup"><span data-stu-id="c9f71-158">String</span></span> | <span data-ttu-id="c9f71-159">LaunchURI ou serviço.</span><span class="sxs-lookup"><span data-stu-id="c9f71-159">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="c9f71-160">id</span><span class="sxs-lookup"><span data-stu-id="c9f71-160">id</span></span>| <span data-ttu-id="c9f71-161">String</span><span class="sxs-lookup"><span data-stu-id="c9f71-161">String</span></span> | <span data-ttu-id="c9f71-162">A ID de um comando que foi enviado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c9f71-162">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="c9f71-163">actionStatus</span><span class="sxs-lookup"><span data-stu-id="c9f71-163">actionStatus</span></span> | <span data-ttu-id="c9f71-164">String</span><span class="sxs-lookup"><span data-stu-id="c9f71-164">String</span></span> | <span data-ttu-id="c9f71-165">O [status](get-device-command-status.md) de um comando.</span><span class="sxs-lookup"><span data-stu-id="c9f71-165">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="c9f71-166">erro</span><span class="sxs-lookup"><span data-stu-id="c9f71-166">error</span></span>| <span data-ttu-id="c9f71-167">String</span><span class="sxs-lookup"><span data-stu-id="c9f71-167">String</span></span>| <span data-ttu-id="c9f71-168">Quaisquer erros associados à solicitação do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="c9f71-168">Any errors associated with the request from the target application.</span></span> |

## <a name="examples"></a><span data-ttu-id="c9f71-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c9f71-169">Examples</span></span>

### <a name="example-1-launch-uri"></a><span data-ttu-id="c9f71-170">Exemplo 1: URI de lançamento</span><span class="sxs-lookup"><span data-stu-id="c9f71-170">Example 1: Launch URI</span></span>

<span data-ttu-id="c9f71-171">Este é um exemplo de uma solicitação LaunchURI; ele iniciará um URI ou um aplicativo no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="c9f71-171">The following is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="c9f71-172">Para iniciar um URI ou um aplicativo, emita uma POSTAgem usando a ID do dispositivo (obtido de uma chamada GET ativada `me/devices` ).</span><span class="sxs-lookup"><span data-stu-id="c9f71-172">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="c9f71-173">Defina os parâmetros de *tipo* como *LaunchURI* e forneça um valor de URI como https://bing.com .</span><span class="sxs-lookup"><span data-stu-id="c9f71-173">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="c9f71-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f71-174">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```
#### <a name="response"></a><span data-ttu-id="c9f71-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9f71-175">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


### <a name="example-2-app-service"></a><span data-ttu-id="c9f71-176">Exemplo 2: serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9f71-176">Example 2: App service</span></span>

<span data-ttu-id="c9f71-177">O exemplo a seguir mostra como consultar um serviço de aplicativo em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c9f71-177">The following example shows how to query an app service on a device.</span></span> <span data-ttu-id="c9f71-178">Para usar um serviço de aplicativo, você deve fazer uma chamada POST usando a ID do dispositivo (obtido de uma chamada GET ativada `me/devices` ).</span><span class="sxs-lookup"><span data-stu-id="c9f71-178">To use an app service, you must do a POST call using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="c9f71-179">Para usar o exemplo a seguir, você deve instalar o [aplicativo Roma](https://aka.ms/romanapp) no seu dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="c9f71-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="c9f71-180">Várias propriedades adicionais devem ser definidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="c9f71-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="c9f71-181">O *tipo* deve ser definido *como serviço*, *AppServiceName* deve ser definido como o nome do serviço de aplicativo definido no aplicativo, *PackageFamilyName* deve ser definido como o nome da família de pacote definido no manifesto do aplicativo e a *carga* contém as chaves e os valores para o serviço que você está chamando no aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="c9f71-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="c9f71-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f71-182">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a><span data-ttu-id="c9f71-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9f71-183">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
