---
title: "allowedRemoteAssistanceActions enum type" description: "Flags enumeration indicating whether a helper can establish a "View screen", "Take full control" and "Elevation" remote assistance action with a device or sharer" author: "dougeby" ms.localizationpriority: medium ms.prod: "intune" doc_type: enumPageType
---

# <a name="allowedremoteassistanceactions-enum-type"></a>tipo de número allowedRemoteAssistanceActions

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Enumeração de sinalizadores indicando se um auxiliar pode estabelecer uma ação de assistência remota "Exibir tela", "Assumir controle total" e "Elevação" com um dispositivo ou sharer

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|viewScreen|1|O auxiliar pode exibir a tela do dispositivo do sharer|
|takeFullControl|2|O auxiliar pode assumir o controle total do dispositivo do sharer|
|elevation|4 |O auxiliar pode assumir o controle total do dispositivo do sharer com privilégios elevados|



