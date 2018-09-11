# <a name="devicethreatprotectionlevel-enum-type"></a>tipo enumerado deviceThreatProtectionLevel

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Níveis de proteção de ameaça de dispositivo para a API de Proteção de ameaça do dispositivo.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unavailable|0|Valor padrão. Não o use.|
|secured|1|Requisito de nível de ameaça de dispositivo: protegido. Esse é o nível mais seguro e indica que nenhuma ameaça foi encontrada no dispositivo.|
|low|2|Requisito de nível de proteção contra ameaças de dispositivo: baixo. Baixo indica uma gravidade de ameaça que apresenta um risco mínimo para o dispositivo ou para os dados do dispositivo.|
|medium|3|Requisito de nível de proteção contra ameaças de dispositivo: médio. Médio indica uma gravidade de ameaça que apresenta risco moderado para o dispositivo ou para os dados do dispositivo.|
|high|4|Requisito de nível de proteção contra ameaças de dispositivo: alto. Alto indica uma gravidade de ameaça que apresenta um risco grave para o dispositivo ou para os dados do dispositivo.|
|notSet|10|Requisito de nível de proteção contra ameaças do dispositivo: não definido. Não definido indica que não há nenhum requisito para que o dispositivo atenda a um nível de proteção contra ameaças.|








