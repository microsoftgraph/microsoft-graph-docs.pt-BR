---
title: Tipo de recurso macOSPrivacyAccessControlItem
description: Representa preferências de privacidade por processo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 158729518b47be682e00bea9d77b8a7308c9d4b1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789633"
---
# <a name="macosprivacyaccesscontrolitem-resource-type"></a>Tipo de recurso macOSPrivacyAccessControlItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa preferências de privacidade por processo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do aplicativo, processo ou executável.|
|identificador|Cadeia de caracteres|A ID do pacote ou o caminho do aplicativo, processo ou executável.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Uma ID de pacote é usada para identificar um aplicativo. Um caminho é usado para identificar um processo ou executável. Os valores possíveis são: `bundleID` e `path`.|
|codeRequirement|Cadeia de caracteres|Insira o requisito de código, que pode ser obtido com o comando 'codesign –display -r –' no aplicativo Terminal. Inclua tudo depois de '=>'.|
|staticCodeValidation|Boleano|Valida estáticamente o requisito de código. Use essa configuração se o processo invalidar sua assinatura de código dinâmico.|
|blockCamera|Boleano|Bloquear o acesso ao aplicativo câmera.|
|blockMicrophone|Booliano|Bloquear o acesso ao microfone.|
|blockScreenCapture|Boleano|Impedir que o aplicativo captura o conteúdo da exibição do sistema. Requer macOS 10.15 ou posterior.|
|blockListenEvent|Booliano|Impedir que o aplicativo ou o processo ouça eventos de dispositivos de entrada, como mouse, teclado e trackpad. Requer macOS 10.15 ou posterior.|
|speechRecognition|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso à instalação de reconhecimento de fala do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|acessibilidade|[enablement](../resources/intune-shared-enablement.md)|Permitir que o aplicativo ou o processo controle o Mac por meio do subsistema Acessibilidade. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|addressBook|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso às informações de contato gerenciadas por Contatos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|calendar|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso às informações de evento gerenciadas pelo Calendário. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|lembretes|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso a informações gerenciadas por Lembretes. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|photos|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso a imagens gerenciadas por Fotos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|mediaLibrary|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso à música e à biblioteca de mídia. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|fileProviderPresence|[enablement](../resources/intune-shared-enablement.md)|Permitir que o aplicativo ou o processo acesse arquivos gerenciados pela extensão do provedor de arquivos de outro aplicativo. Requer macOS 10.15 ou posterior. . Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyAllFiles|[enablement](../resources/intune-shared-enablement.md)|Controlar o acesso a todos os arquivos protegidos em um dispositivo. Os arquivos podem estar em locais como emails, mensagens, aplicativos e configurações administrativas. Aplique essa configuração com cuidado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicySystemAdminFiles|[enablement](../resources/intune-shared-enablement.md)|Permitir que o aplicativo ou o processo acesse arquivos usados na administração do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDesktopFolder|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso à pasta Área de Trabalho. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDocumentsFolder|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso à pasta Documentos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDownloadsFolder|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso à pasta Downloads. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyNetworkVolumes|[enablement](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso aos volumes de rede. Requer macOS 10.15 ou posterior. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyRemovableVolumes|[enablement](../resources/intune-shared-enablement.md)|Controle o acesso a volumes removíveis no dispositivo, como um disco rígido externo. Requer macOS 10.15 ou posterior. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|postEvent|[enablement](../resources/intune-shared-enablement.md)|Controle o acesso às APIs CoreGraphics, que são usadas para enviar CGEvents para o fluxo de eventos do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|appleEventsAllowedReceivers|[Coleção macOSAppleEventReceiver](../resources/intune-deviceconfig-macosappleeventreceiver.md)|Permitir ou negar que o aplicativo ou processo envie um evento Apple restrito para outro aplicativo ou processo. Você precisará saber o identificador, o tipo de identificador e o requisito de código do aplicativo ou processo de recebimento. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSPrivacyAccessControlItem",
  "displayName": "String",
  "identifier": "String",
  "identifierType": "String",
  "codeRequirement": "String",
  "staticCodeValidation": true,
  "blockCamera": true,
  "blockMicrophone": true,
  "blockScreenCapture": true,
  "blockListenEvent": true,
  "speechRecognition": "String",
  "accessibility": "String",
  "addressBook": "String",
  "calendar": "String",
  "reminders": "String",
  "photos": "String",
  "mediaLibrary": "String",
  "fileProviderPresence": "String",
  "systemPolicyAllFiles": "String",
  "systemPolicySystemAdminFiles": "String",
  "systemPolicyDesktopFolder": "String",
  "systemPolicyDocumentsFolder": "String",
  "systemPolicyDownloadsFolder": "String",
  "systemPolicyNetworkVolumes": "String",
  "systemPolicyRemovableVolumes": "String",
  "postEvent": "String",
  "appleEventsAllowedReceivers": [
    {
      "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
      "codeRequirement": "String",
      "identifier": "String",
      "identifierType": "String",
      "allowed": true
    }
  ]
}
```



