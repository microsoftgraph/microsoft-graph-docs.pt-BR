---
title: Criar managedIOSLobApp
description: Cria um novo objeto managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c113c8c76029ee7a0d1c5f3e5d0b1d0ab5f31bba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987071"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="0c9b5-103">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="0c9b5-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="0c9b5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c9b5-105">Cria um novo objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c9b5-105">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c9b5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c9b5-106">Prerequisites</span></span>
<span data-ttu-id="0c9b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c9b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c9b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c9b5-109">Permission type</span></span>|<span data-ttu-id="0c9b5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c9b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c9b5-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c9b5-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c9b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c9b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-114">Not supported.</span></span>|
|<span data-ttu-id="0c9b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c9b5-115">Application</span></span>|<span data-ttu-id="0c9b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c9b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c9b5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0c9b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c9b5-118">Request headers</span></span>
|<span data-ttu-id="0c9b5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c9b5-119">Header</span></span>|<span data-ttu-id="0c9b5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0c9b5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c9b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c9b5-121">Authorization</span></span>|<span data-ttu-id="0c9b5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c9b5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c9b5-123">Accept</span></span>|<span data-ttu-id="0c9b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0c9b5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c9b5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c9b5-125">Request body</span></span>
<span data-ttu-id="0c9b5-126">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-126">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="0c9b5-127">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-127">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="0c9b5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c9b5-128">Property</span></span>|<span data-ttu-id="0c9b5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c9b5-129">Type</span></span>|<span data-ttu-id="0c9b5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c9b5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c9b5-131">id</span><span class="sxs-lookup"><span data-stu-id="0c9b5-131">id</span></span>|<span data-ttu-id="0c9b5-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-132">String</span></span>|<span data-ttu-id="0c9b5-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-133">Key of the entity.</span></span> <span data-ttu-id="0c9b5-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0c9b5-135">displayName</span></span>|<span data-ttu-id="0c9b5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-136">String</span></span>|<span data-ttu-id="0c9b5-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0c9b5-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-139">descrição</span><span class="sxs-lookup"><span data-stu-id="0c9b5-139">description</span></span>|<span data-ttu-id="0c9b5-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-140">String</span></span>|<span data-ttu-id="0c9b5-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-141">The description of the app.</span></span> <span data-ttu-id="0c9b5-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-143">publisher</span><span class="sxs-lookup"><span data-stu-id="0c9b5-143">publisher</span></span>|<span data-ttu-id="0c9b5-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-144">String</span></span>|<span data-ttu-id="0c9b5-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-145">The publisher of the app.</span></span> <span data-ttu-id="0c9b5-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0c9b5-147">largeIcon</span></span>|[<span data-ttu-id="0c9b5-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0c9b5-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0c9b5-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0c9b5-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c9b5-151">createdDateTime</span></span>|<span data-ttu-id="0c9b5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c9b5-152">DateTimeOffset</span></span>|<span data-ttu-id="0c9b5-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-153">The date and time the app was created.</span></span> <span data-ttu-id="0c9b5-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c9b5-155">lastModifiedDateTime</span></span>|<span data-ttu-id="0c9b5-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c9b5-156">DateTimeOffset</span></span>|<span data-ttu-id="0c9b5-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-157">The date and time the app was last modified.</span></span> <span data-ttu-id="0c9b5-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0c9b5-159">isFeatured</span></span>|<span data-ttu-id="0c9b5-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="0c9b5-160">Boolean</span></span>|<span data-ttu-id="0c9b5-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0c9b5-162">privacyInformationUrl</span></span>|<span data-ttu-id="0c9b5-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-163">String</span></span>|<span data-ttu-id="0c9b5-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-164">The privacy statement Url.</span></span> <span data-ttu-id="0c9b5-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0c9b5-166">informationUrl</span></span>|<span data-ttu-id="0c9b5-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-167">String</span></span>|<span data-ttu-id="0c9b5-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-168">The more information Url.</span></span> <span data-ttu-id="0c9b5-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-170">owner</span><span class="sxs-lookup"><span data-stu-id="0c9b5-170">owner</span></span>|<span data-ttu-id="0c9b5-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-171">String</span></span>|<span data-ttu-id="0c9b5-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-172">The owner of the app.</span></span> <span data-ttu-id="0c9b5-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-174">developer</span><span class="sxs-lookup"><span data-stu-id="0c9b5-174">developer</span></span>|<span data-ttu-id="0c9b5-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-175">String</span></span>|<span data-ttu-id="0c9b5-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-176">The developer of the app.</span></span> <span data-ttu-id="0c9b5-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-178">Observações</span><span class="sxs-lookup"><span data-stu-id="0c9b5-178">notes</span></span>|<span data-ttu-id="0c9b5-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-179">String</span></span>|<span data-ttu-id="0c9b5-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-180">Notes for the app.</span></span> <span data-ttu-id="0c9b5-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c9b5-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="0c9b5-182">publishingState</span></span>|[<span data-ttu-id="0c9b5-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0c9b5-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0c9b5-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-184">The publishing state for the app.</span></span> <span data-ttu-id="0c9b5-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0c9b5-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c9b5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0c9b5-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0c9b5-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="0c9b5-188">appAvailability</span></span>|[<span data-ttu-id="0c9b5-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="0c9b5-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="0c9b5-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-190">The Application's availability.</span></span> <span data-ttu-id="0c9b5-191">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c9b5-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="0c9b5-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="0c9b5-193">version</span><span class="sxs-lookup"><span data-stu-id="0c9b5-193">version</span></span>|<span data-ttu-id="0c9b5-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-194">String</span></span>|<span data-ttu-id="0c9b5-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-195">The Application's version.</span></span> <span data-ttu-id="0c9b5-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="0c9b5-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0c9b5-197">committedContentVersion</span></span>|<span data-ttu-id="0c9b5-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-198">String</span></span>|<span data-ttu-id="0c9b5-199">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-199">The internal committed content version.</span></span> <span data-ttu-id="0c9b5-200">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0c9b5-201">fileName</span><span class="sxs-lookup"><span data-stu-id="0c9b5-201">fileName</span></span>|<span data-ttu-id="0c9b5-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-202">String</span></span>|<span data-ttu-id="0c9b5-203">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-203">The name of the main Lob application file.</span></span> <span data-ttu-id="0c9b5-204">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0c9b5-205">size</span><span class="sxs-lookup"><span data-stu-id="0c9b5-205">size</span></span>|<span data-ttu-id="0c9b5-206">Int64</span><span class="sxs-lookup"><span data-stu-id="0c9b5-206">Int64</span></span>|<span data-ttu-id="0c9b5-207">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="0c9b5-208">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c9b5-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0c9b5-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="0c9b5-209">bundleId</span></span>|<span data-ttu-id="0c9b5-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-210">String</span></span>|<span data-ttu-id="0c9b5-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-211">The Identity Name.</span></span>|
|<span data-ttu-id="0c9b5-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="0c9b5-212">applicableDeviceType</span></span>|[<span data-ttu-id="0c9b5-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="0c9b5-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="0c9b5-214">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="0c9b5-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c9b5-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0c9b5-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c9b5-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="0c9b5-217">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0c9b5-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0c9b5-218">expirationDateTime</span></span>|<span data-ttu-id="0c9b5-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c9b5-219">DateTimeOffset</span></span>|<span data-ttu-id="0c9b5-220">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-220">The expiration time.</span></span>|
|<span data-ttu-id="0c9b5-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="0c9b5-221">versionNumber</span></span>|<span data-ttu-id="0c9b5-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-222">String</span></span>|<span data-ttu-id="0c9b5-223">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0c9b5-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="0c9b5-224">buildNumber</span></span>|<span data-ttu-id="0c9b5-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9b5-225">String</span></span>|<span data-ttu-id="0c9b5-226">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="0c9b5-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c9b5-227">Response</span></span>
<span data-ttu-id="0c9b5-228">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-228">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c9b5-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c9b5-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c9b5-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c9b5-230">Request</span></span>
<span data-ttu-id="0c9b5-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="0c9b5-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c9b5-232">Response</span></span>
<span data-ttu-id="0c9b5-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c9b5-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



