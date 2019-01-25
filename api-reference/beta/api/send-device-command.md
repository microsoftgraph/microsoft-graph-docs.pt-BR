---
title: Enviar um comando de dispositivo
description: 'Essa API permite que os recursos de projeto Roma para um dispositivo associado a uma conta da Microsoft de comando. Depois de fazer uma chamada GET em `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo. Dois tipos de comandos são suportados: LaunchURI e AppServices. Se você estiver usando LaunchURI, especifique os parâmetros de *tipo* e da *carga* . Para uma chamada de AppService, especifique o '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526239"
---
# <a name="send-device-command"></a><span data-ttu-id="f5da0-107">Enviar um comando de dispositivo</span><span class="sxs-lookup"><span data-stu-id="f5da0-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5da0-108">Essa API permite que os recursos de projeto Roma para um dispositivo associado a uma conta da Microsoft de comando.</span><span class="sxs-lookup"><span data-stu-id="f5da0-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="f5da0-109">Depois de fazer uma chamada GET em `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5da0-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="f5da0-110">Dois tipos de comandos são suportados: LaunchURI e AppServices.</span><span class="sxs-lookup"><span data-stu-id="f5da0-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="f5da0-111">Se você estiver usando LaunchURI, especifique os parâmetros de *tipo* e da *carga* .</span><span class="sxs-lookup"><span data-stu-id="f5da0-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="f5da0-112">Para uma chamada de AppService, especifique o *tipo*, *carga*, *packageFamilyName*e *appServiceName* parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f5da0-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5da0-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5da0-113">Permissions</span></span>

<span data-ttu-id="f5da0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5da0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f5da0-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5da0-116">Permission type</span></span>      | <span data-ttu-id="f5da0-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5da0-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5da0-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5da0-118">Delegated (work or school account)</span></span> | <span data-ttu-id="f5da0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5da0-119">Not supported.</span></span>    |
|<span data-ttu-id="f5da0-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5da0-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5da0-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f5da0-121">Device.Command</span></span>    |
|<span data-ttu-id="f5da0-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5da0-122">Application</span></span> | <span data-ttu-id="f5da0-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5da0-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5da0-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5da0-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="f5da0-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5da0-125">Request headers</span></span>


| <span data-ttu-id="f5da0-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5da0-126">Header</span></span> |<span data-ttu-id="f5da0-127">Valor</span><span class="sxs-lookup"><span data-stu-id="f5da0-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="f5da0-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5da0-128">Authorization</span></span>| <span data-ttu-id="f5da0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5da0-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f5da0-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5da0-131">Accept</span></span> | <span data-ttu-id="f5da0-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f5da0-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5da0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5da0-133">Request body</span></span>

<span data-ttu-id="f5da0-134">No corpo da solicitação, fornece uma representação JSON das propriedades do comando.</span><span class="sxs-lookup"><span data-stu-id="f5da0-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="f5da0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5da0-135">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="f5da0-136">Command Properties</span><span class="sxs-lookup"><span data-stu-id="f5da0-136">Command properties</span></span> 

|<span data-ttu-id="f5da0-137">**Name**</span><span class="sxs-lookup"><span data-stu-id="f5da0-137">**Name**</span></span>|<span data-ttu-id="f5da0-138">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="f5da0-138">**Type**</span></span>|<span data-ttu-id="f5da0-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f5da0-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="f5da0-140">payload</span><span class="sxs-lookup"><span data-stu-id="f5da0-140">payload</span></span> | <span data-ttu-id="f5da0-141">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="f5da0-141">microsoft.graph.json</span></span>| <span data-ttu-id="f5da0-142">Carga para enviar para um serviço do aplicativo ou iniciar um URI em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5da0-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="f5da0-143">responsePayload</span><span class="sxs-lookup"><span data-stu-id="f5da0-143">responsePayload</span></span> | <span data-ttu-id="f5da0-144">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="f5da0-144">microsoft.graph.json</span></span>| <span data-ttu-id="f5da0-145">Carga retornado do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f5da0-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="f5da0-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="f5da0-146">postBackURI</span></span> | <span data-ttu-id="f5da0-147">String</span><span class="sxs-lookup"><span data-stu-id="f5da0-147">String</span></span> | <span data-ttu-id="f5da0-148">URI para enviar notificações subsequentes das atualizações de volta de postagem.</span><span class="sxs-lookup"><span data-stu-id="f5da0-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="f5da0-149">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="f5da0-149">packageFamilyName</span></span> | <span data-ttu-id="f5da0-150">String</span><span class="sxs-lookup"><span data-stu-id="f5da0-150">String</span></span> | <span data-ttu-id="f5da0-151">Nome da família Windows pacote de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f5da0-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="f5da0-152">appServiceName</span><span class="sxs-lookup"><span data-stu-id="f5da0-152">appServiceName</span></span> | <span data-ttu-id="f5da0-153">String</span><span class="sxs-lookup"><span data-stu-id="f5da0-153">String</span></span> | <span data-ttu-id="f5da0-154">Nome do serviço de aplicativo definido pelo aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="f5da0-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="f5da0-155">Será necessário se lançar um serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f5da0-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="f5da0-156">type</span><span class="sxs-lookup"><span data-stu-id="f5da0-156">type</span></span>| <span data-ttu-id="f5da0-157">String</span><span class="sxs-lookup"><span data-stu-id="f5da0-157">String</span></span> | <span data-ttu-id="f5da0-158">LaunchURI ou AppService.</span><span class="sxs-lookup"><span data-stu-id="f5da0-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="f5da0-159">id</span><span class="sxs-lookup"><span data-stu-id="f5da0-159">id</span></span>| <span data-ttu-id="f5da0-160">String</span><span class="sxs-lookup"><span data-stu-id="f5da0-160">String</span></span> | <span data-ttu-id="f5da0-161">A identificação de um comando que foi enviado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5da0-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="f5da0-162">actionStatus</span><span class="sxs-lookup"><span data-stu-id="f5da0-162">actionStatus</span></span> | <span data-ttu-id="f5da0-163">String</span><span class="sxs-lookup"><span data-stu-id="f5da0-163">String</span></span> | <span data-ttu-id="f5da0-164">O [status](get-device-command-status.md) de um comando.</span><span class="sxs-lookup"><span data-stu-id="f5da0-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="f5da0-165">erro</span><span class="sxs-lookup"><span data-stu-id="f5da0-165">error</span></span>| <span data-ttu-id="f5da0-166">String</span><span class="sxs-lookup"><span data-stu-id="f5da0-166">String</span></span>| <span data-ttu-id="f5da0-167">Quaisquer erros associados à solicitação do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="f5da0-167">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="f5da0-168">Exemplo URI de início</span><span class="sxs-lookup"><span data-stu-id="f5da0-168">Launch URI example</span></span>

<span data-ttu-id="f5da0-169">Aqui está um exemplo de uma solicitação de LaunchURI; ele iniciará um URI ou um aplicativo no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f5da0-169">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="f5da0-170">Para iniciar um aplicativo ou um URI, emitir um POST usando a ID do dispositivo (obtido fazendo uma chamada GET em `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="f5da0-170">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="f5da0-171">Definir os parâmetros de *tipo* para *LaunchURI* e fornecer um valor URI, tais como https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="f5da0-171">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="f5da0-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5da0-172">Request</span></span>

<span data-ttu-id="f5da0-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5da0-173">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="f5da0-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5da0-174">Response</span></span> 

<span data-ttu-id="f5da0-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5da0-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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


## <a name="app-service-example"></a><span data-ttu-id="f5da0-176">Exemplo de aplicativo do serviço</span><span class="sxs-lookup"><span data-stu-id="f5da0-176">App service example</span></span>

<span data-ttu-id="f5da0-177">Aqui está um exemplo de uma consulta de um serviço de aplicativo em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5da0-177">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="f5da0-178">Para usar um serviço de aplicativo, você deve fazer uma chamada de POSTAGEM usando a id do dispositivo (obtido fazendo uma chamada GET em `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="f5da0-178">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="f5da0-179">Para usar o exemplo a seguir, você deve instalar o [aplicativo Roma](https://aka.ms/romanapp) no seu dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f5da0-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="f5da0-180">Várias outras propriedades devem ser definidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="f5da0-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="f5da0-181">*Tipo* deve ser definida como *AppService*, *AppServiceName* deve ser definida com o nome da definida no aplicativo de serviço do aplicativo, *PackageFamilyName* deve ser definida como o nome da família de pacote definido no manifesto do aplicativo e *carga* contém as chaves e valores para o serviço que você está chamando dentro do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="f5da0-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="f5da0-182">Solicitar</span><span class="sxs-lookup"><span data-stu-id="f5da0-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f5da0-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5da0-183">Response</span></span>

<span data-ttu-id="f5da0-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5da0-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/send-device-command.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
